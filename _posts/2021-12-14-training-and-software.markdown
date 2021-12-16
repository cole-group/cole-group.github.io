---
layout: post
title:  "Training & Software Resources"
date:   2021-12-14
---

In this post, I'll link to a few training materials and software packages that might be useful to new starters in our group (or elsewhere). I intend for this to be updated regularly, so please feel free to suggest changes or additions, particularly if links break. A big thank you to everyone that has made these resources available online, we find them invaluable!


## Workshops

[CCP-BioSim.][ccpbiosim] Excellent set of training modules and Youtube channel. Subjects include biomolecular dynamics, FESetup, BioSimSpace and Python for biomolecular modelling.

[RSC Chemical Information and Computer Applications Group.][rsc-cicag] Highly recommended series of webinars on open source tools for chemistry, including cheminformatics, docking (gnina), chimeraX and pymol.

[Bespoke-fit.][bespokefit] A workshop describing the use of Open Force Field's [bespoke-fit package][bespokefit-github] for fitting molecule-specific torsion parameters, given by our own Josh Horton.

[TeachOpenCADD.][teachopencadd] Really useful set of talktorials on the use of open source cheminformatics tools for computer-aided drug design.

[The Alan Turing Institute][turing] offers online [Introduction to Research Data Science][turing1] ([github repo][turing-github1]) and [Software Engineering][turing2] ([github repo][turing-github2]) courses.

[Molecular Software Sciences Institute.][molssi] Highly recommended workshops on topics including programming and molecular modelling. 

[The AI3SD network][ai3sd1] have kindly made available a series of recorded research seminars, as well as a [Skills 4 Scientists][ai3sd2] series (including research data management, python, version control, ethics, and career development).


## Research Software

[QUBEKit.][qubekit] Our own Quantum Mechanical Bespoke Force Field Derivation Toolkit, by Chris Ringrose and Josh Horton. More tutorials coming soon, watch this space!

[Open Force Field.][openff] We're very happy to be working with the Open Force Field initiative, and we make extensive use of their software infrastructure in our work. A good place to start is with the [documentation examples][openff1] on building and interacting with molecules, and a [set of notebooks][openff2], which show how to use the toolkit to parameterise a system and run a short simulation in OpenMM.

[OpenMM.][openmm] All of our atomistic molecular dynamics simulations are performed through OpenMM. A few tutorials are available [here][openmm-tut], with more to follow I believe.

[BioSimSpace / SOMD.][bss] Python framework for biomolecular simulation, includes a [set of tutorials][bss-tut] for common simulation types. [Our own tutorials][somd-qube] written with Julien Michel's lab show how to use SOMD in protein-ligand binding and hydration free energy calculations with different force fields.

[RDKit.][rdkit] Open source cheminformatics toolkit, which we use in virtually all our workflows. You'll find many tutorials online, including [Getting started with RDKit in python][rdkit-tut] and introductory youtube tutorials by Jan Jensen: [Tutorial 1][rdkit1]; [Tutorial 2][rdkit2].

[QCArchive.][qcarchive] Josh In particular has done a lot of work with MolSSI's quantum chemistry archive, which is resource for compiling and sharing QM data. Lots of documentation is available, including for [QCengine][qcengine], a quantum chemistry program executor and IO standardiser for quantum chemistry.

[ONETEP.][onetep] Several of our projects involve large-scale DFT calculations, often working with the ONETEP community. Frequent workshops are run and [tutorials][onetep-tut] are available online.

[DeLinker.][delinker] Deep generative models for 3D linker design. We've found this to be very promising in fragment-based design projects.

[Gnina.][gnina] We don't use docking very often to be honest, but do like the ease-of-use and promising accuracy of gnina. David Koes also has an excellent [webinar][gnina-tut] describing its use.

[DeepChem.][deepchem] Open-source toolchain demonstrating the use of deep learning in drug discovery, materials science, quantum chemistry, and biology, with [extensive online tutorials][deepchem-tut].


## Miscellaneous

[Learning Scientific Programming with Python.][python] The course textbook for my undergraduate Python classes (Newcastle students, feel free to message me for access to course materials). Textbook should be available through Newcastle University library.

[Deep Learning for Molecules and Materials.][ml] I'm only on Chapter 2 so far, but this looks like a really good online textbook by Andrew White, with code examples.

[In Silico Medicinal Chemistry: Computational Methods to Support Drug Design.][brown] Book by Nathan Brown on computational tools for drug design. Should be available through Newcastle University library.




[ccpbiosim]: https://www.ccpbiosim.ac.uk/training
[openff]: https://openforcefield.org
[openff1]: https://open-forcefield-toolkit.readthedocs.io/en/0.10.1/users/molecule_cookbook.html
[openff2]: https://github.com/openforcefield/openff-toolkit/tree/master/examples#examples-using-smirnoff-with-the-toolkit
[bespokefit]: https://www.youtube.com/watch?v=xQ8pnYcmWSU
[bespokefit-github]: https://github.com/openforcefield/openff-bespokefit
[teachopencadd]: https://projects.volkamerlab.org/teachopencadd/
[bss]: https://biosimspace.org
[bss-tut]: https://github.com/michellab/BioSimSpaceTutorials
[somd-qube]: https://github.com/cole-group/QUBE-SOMD-paper
[rsc-cicag]: https://www.youtube.com/c/RSCCICAG/videos
[brown]: https://pubs.rsc.org/en/content/ebook/978-1-78262-163-8
[python]: https://www-cambridge-org.libproxy.ncl.ac.uk/core/books/learning-scientific-programming-with-python/3D264483BC7B380A3059B3861C661237
[turing]: https://www.turing.ac.uk
[turing-github1]: https://github.com/alan-turing-institute/rds-course
[turing1]: https://alan-turing-institute.github.io/rds-course/index.html
[turing2]: https://alan-turing-institute.github.io/rse-course/html/index.html
[turing-github2]: https://github.com/alan-turing-institute/rse-course
[molssi]: http://education.molssi.org/resources.html#programming
[qubekit]: https://github.com/qubekit/QUBEKit
[openmm]: https://openmm.org
[openmm-tut]: https://openmm.org/tutorials
[onetep]: https://www.onetep.org/Main/HomePage
[onetep-tut]: https://www.onetep.org/Main/Tutorials
[rdkit]: https://www.rdkit.org/docs/index.html
[rdkit-tut]: https://www.rdkit.org/docs/GettingStartedInPython.html
[rdkit1]: https://www.youtube.com/watch?v=ERvUf_lNopo&t=0s
[rdkit2]: https://www.youtube.com/watch?v=3qzZbaUzo9M
[delinker]: https://github.com/oxpig/DeLinker
[qcarchive]: https://qcarchive.molssi.org
[qcengine]: http://docs.qcarchive.molssi.org/projects/QCEngine/en/stable/
[gnina]: https://github.com/gnina/gnina
[gnina-tut]: https://www.youtube.com/watch?v=MG3Srzi5kZ0
[ml]: https://dmol.pub/intro.html
[deepchem]: https://deepchem.io
[deepchem-tut]: https://github.com/deepchem/deepchem/tree/master/examples/tutorials
[ai3sd1]: https://www.ai3sd.org/ai3sd-online-seminar-series/
[ai3sd2]: https://www.ai3sd.org/ai3sd-online-seminar-series/skills-4-scientists-seminar-series-2021/
