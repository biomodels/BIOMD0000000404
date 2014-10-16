# BIOMD0000000404: Bray1993_chemotaxis

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000404.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000404.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000404 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


This version of the model is very close to the version described in the paper
with one exception: the binding of aspartate to the various receptor
complexes, as well as the formation of the different complexes are modeled
using chemical kinetics (mass action law), rather than instant equilibrium.
The qualitative behaviour of the model is unchanged. Note that in order to
quantitatively replicate the figure 8b, and in particular to have a basal bias
of 0.7, we have to change the rate constant of the aspartate-triggered
dephosphorylation of CheY from 59000 to 70000. The peaks have then slightly
different values.

This model originates from BioModels Database: A Database of Annotated
Published Models (http://www.ebi.ac.uk/biomodels/). It is copyright (c)
2005-2012 The BioModels.net Team.  
For more information see the [terms of
use](http://www.ebi.ac.uk/biomodels/legal.html) .  
To cite BioModels Database, please use: [Li C, Donizelli M, Rodriguez N,
Dharuri H, Endler L, Chelliah V, Li L, He E, Henry A, Stefan MI, Snoep JL,
Hucka M, Le Novère N, Laibe C (2010) BioModels Database: An enhanced, curated
and annotated resource for published quantitative kinetic models. BMC Syst
Biol., 4:92.](http://www.ncbi.nlm.nih.gov/pubmed/20587024)


