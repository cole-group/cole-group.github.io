---
layout: post
title:  "Using QUBEKit as an API"
date:   2022-08-03
---

[QUBEKit][qubekitlink] is easy to use as an Application Programming Interface (API) for two key reasons: the persistent molecule object and the separated stages. By initialising a molecule from a file or SMILES string, it can then be passed to any of QUBEKit’s stages to be operated on. The coordinates can be optimised, bond and angle parameters can be calculated, virtual sites can be added, all in the same way. For example, the following code could be used to fit virtual sites to a molecule, given only a pdb file and some charge data from Chargemol:





To include an image in your post:

![QUBEKit logo](/assets/QuBeKit.png)

or [link to it in the text](/assets/QuBeKit.png).


{% highlight ruby %}
from qubekit.charges import DDECCharges, ExtractChargeData
from qubekit.molecules import Ligand
from qubekit.nonbonded import VirtualSites
from qubekit.parametrisation import OpenFF

# Load the molecule into QUBEKit from file.
molecule = Ligand.from_file("methylisocyanate.pdb") # Generate basic parameters using OpenFF.
OpenFF().run(molecule)

# Extract charge data and save to be used in the virtual sites fit.
ddec_file_path = "ChargeMol"
ddec_version = 6

ExtractChargeData.extract_charge_data_chargemol(
    molecule, ddec_file_path, ddec_version
)

# Apply symmetry to the reference data (optional).
DDECCharges.apply_symmetrisation(molecule) # Fit virtual sites to the molecule.
VirtualSites().run(molecule)

# Write the force field parameters to file.
molecule.write_parameters("methylisocyanate.xml")
{% endhighlight %}

## How to find out more

Check out the [QUBEKit docs][qubekitlink] for more info on how to get the most out of QUBEKit.

[qubekitlink]: https://github.com/qubekit/QUBEKit

