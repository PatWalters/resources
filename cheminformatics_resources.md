### **A Highly Opinionated List of Open Source Cheminformatics Resources**

This is a list of some of the Cheminformatics resources that I use.  Rather than a long list of links, this is an annotated collection of tools that I use regularly.  The order in which things are presented is a representation of my scattered thought processes and does not imply relative importance.  These are the views of one highly opinionated guy.  Your mileage may vary. 

### Getting Started

[Bonn Workshop](https://github.com/PatWalters/workshop) - I taught a 2 day hands-on Cheminformatics workshop at the University of Bonn in the summer of 2019.  The Jupyter notebooks I used for this workshop are available on [GitHub](https://github.com/PatWalters/workshop).  They can be run on [Binder](https://mybinder.org/v2/gh/PatWalters/workshop/master) without installing any software. 

[TeachOpenCADD](https://github.com/volkamerlab/TeachOpenCADD) - This is a great set of tutorials from Andrea Volkamer's group that use Open Source software to teach Computer-Aided Drug Design concepts including molecular similarity, applications of machine learning, and pharmacophore analysis. 

[The RDKit Cookbook](https://www.rdkit.org/docs/Cookbook.html) - This is a terrific resource that provides "recipes" for a number of common tasks. 

[RDKitTutorial](https://github.com/suneelbvs/rdkit_tutorials) - A nice set of Jupyter notebooks from Suneel Kumar BVS with examples of basic molecule manipulations using the RDKit. 

[Machine Learning Mastery](https://machinelearningmastery.com/blog/) - Jason Brownlee writes about machine learning in a very practical, easy to understand fashion.  I've learned so much from his blogs.  I also highly recommend his eBooks.

[Deep Learning for the Life Sciences](https://www.oreilly.com/library/view/deep-learning-for/9781492039822/) - A shameless plug for a book I cowrote.  I really do think this is a good resource that is chock full of useful code examples.  Code from the book can be found [here](https://github.com/deepchem/DeepLearningLifeSciences). 

### **Blogs**

[Practical Cheminformatics](https://practicalcheminformatics.blogspot.com/) - This is a blog where I post once a month or so. These posts typically contain code that demonstrates various aspects of cheminformatics; clustering, machine learning, data visualization, etc. I occasionally throw in posts containing opinions on things like AI and getting a job. 

[Is Life Worth Living](https://iwatobipen.wordpress.com/) - A great blog from Iwatobipen (aka pen), whose posts are chock full of great code examples.  Pen always seems to be up on the latest methods and posts interesting examples on a variety of topics ranging from quantum chemistry to machine learning. 

[The RDKit Blog](http://rdkit.blogspot.com/) - Greg Landrum is the primary contributor to, and BDFL, of the RDKit.  In addition to the latest and greatest features in the RDKit, Greg's posts also touch on a number of key issues in Cheminformatics, such as dealing with unbalanced datasets and the impact of fingerprint folding on similarity searching. 

[Reverie Labs Engineering Blog](https://blog.reverielabs.com/) - The gang at Reverie Labs is doing some of the best work on applying machine learning in drug discovery.  Their blog provides useful insights for those applying machine learning at scale. 

[The OpenBench Blog](https://opnbnch.substack.com/) - A number of thoughtful posts on ADME modeling and the ways that we validate models. 

[Cheminformania](http://www.cheminformania.com/) - A set of very practical posts by Esben Jannik Bjerrum and friends that primarily focus on the applications of deep learning in drug discovery.  These posts provide several useful code examples.

### **Python Tools**

**General**

[Jupyter Notebooks](https://jupyter.org/) - Perhaps the greatest scientific development of my lifetime.  I don't know how I ever did science without a Jupyter notebook.  If you don't know what this is, stop reading now and click on the link.  In a nutshell, Jupyter notebooks provide a way of integrating documentation and workflows into a simple, easy to use tool.  Yes, I know that there are some minor annoyances (executing cells out of order), but these can be overcome with a little discipline.  Jupyter notebooks have become my standard means of sharing code with colleagues and with the community.  As the sticker on my laptop says "For the times when your Boss asks for Documentation".

[JupyterLab](https://blog.jupyter.org/jupyterlab-is-ready-for-users-5a6f039b8906) - I know I should use JupyterLab more than I do. It provides some convenient ways of enhancing the standard Jupyter notebook workflow, but JupyterLab also has a nasty habit of not working with some Jupyter extensions. 


**Python Libraries I Can't Live Without**

[Pandas](https://pandas.pydata.org/) - I spent about a dozen years as an R programmer.  During that time I got used to thinking about data tables as dataframes in memory.  Pandas provides an incredibly robust, fast, and well thought out set up tools for dealing with tabular data.  If you want to do something with a table, Pandas probably already knows how.  Thanks to efforts by the RDKit community, we can also store and display chemical structures in Pandas dataframes using the [PandasTools](https://www.rdkit.org/docs/source/rdkit.Chem.PandasTools.html) library. 

[numpy](https://numpy.org/) - Need to do any sort of operation with vectors or matrices? Numpy makes it fast and easy.  

[tqdm](https://github.com/tqdm/tqdm) - I'm impatient, I admit it.  I want to know that my code is running and when it will finish.  In order to do this, I need a progress bar.  I don't know of an easier way to put a progress bar in a Python script than tqdm.  This library works seamlessly in both command line scripts and Jupyter notebooks.

[docopt](https://github.com/docopt/docopt) - Occasionally I have to put a commandline interface on a Python script and I need a library to simplify this process.  There are a lot of libraries for commandline processing, this is the one I like. 


**Python Chemistry Libraries I Can't Live Without**

[The RDKit](https://www.rdkit.org/) - My goto (a command you should never use) library for Open Source Cheminformatics.  The RDKit has a large and supportive community that is always eager to answer questions on the mailing list.  The UGM has become one of the best meetings of the year, and Greg Landrum and friends are making the code better with each release. 

[OpenBabel](http://openbabel.org/wiki/Main_Page) - The OG of Chemistry libraries.  If you want to process some obscure (or not obscure) file format, Open Babel is the way to go.  The library has gotten kind of big, but it has a number of unique capabilities. 

[py3DMol](https://pypi.org/project/py3Dmol/) - This Python wrapper around the 3DMol.js library, written by David Koes, makes it easy to incorporate 3D chemical structures into a Jupyter notebook.  [Greg Landrum](https://nbviewer.jupyter.org/github/greglandrum/rdkit_blog/blob/master/notebooks/Trying%20py3Dmol.ipynb) and [Pen](https://birdlet.github.io/2019/10/02/py3dmol_example/) have some nice blog posts with some simple examples. [I](https://practicalcheminformatics.blogspot.com/2020/05/analyzing-sars-cov-2-main-protease-mpro.html) also have a post showing some uses of Py3DMol. 

[Prody](http://prody.csb.pitt.edu/) - Do you want to work with proteins in Python? Then Prody is the tool for you.  Prody provides tools for reading and processing proteins, as well as implementing techniques like normal mode analysis.  In addition to its many capabilities, Prody is well documented and comes with a ton of examples. 

[MDTraj](https://www.mdtraj.org) - Do you want to be able to process molecular dynamics (MD) trajectories in Python scripts?  Look no further.  MDTraj can read most trajectory formats and provides a wide array of analysis tools.  

[ODDT](https://github.com/oddt/oddt) - The Open Drug Discovery Toolkit builds on the RDKit and/or OpenBabel to provide several useful capabilities including protein-ligand interaction fingerprints and a variety of scoring functions. 

[Descriptasaurus](https://github.com/bp-kelley/descriptastorus) - A handy library from my colleague Brian Kelley that makes it very easy to access molecular descriptors from the RDKit and use them in machine learning models. 

[Pyjanitor](https://github.com/ericmjl/pyjanitor) - A very useful library from Eric Ma that provides a ton of useful features for cleaning up datasets.  Pyjanitor also contains a number of Chemistry specific features that make it easy to generate and integrate molecular descriptors. 

[CReM](https://github.com/DrrDom/crem) - A library for denovo design using chemically reasonable mutations.  CReM is described in [this paper](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-020-00431-w) and [this one](https://pubs.acs.org/doi/10.1021/acs.jcim.0c00792) as well as [this blog post I wrote](https://practicalcheminformatics.blogspot.com/2020/03/building-on-fragments-from-diamondxchem.html). 


 **Molecule Manipulation**
 
[MayaChem Tools](http://www.mayachemtools.org/) - My friend Manish Sud has created a Swiss army knife of Python and Perl Scripts that use Open Source software to perform a wide array of molecule manipulation tasks including [positional scanning](https://practicalcheminformatics.blogspot.com/2020/04/positional-analogue-scanning.html), conformer generation, library enumeration and filtering, R-group decomposition, and numerous other capabilities.  MayaChem Tools also has several scripts for performing analyses with PyMol.  These scripts are useful by themselves or as starting points for you own projects. 


**Data Visualization**

[Seaborn](https://seaborn.pydata.org/) - [Matplotlib](https://matplotlib.org/) is the standard for plotting in Python, it works but doesn't make the most attractive plots.  Seaborn builds on Matplotlib, makes it a bit easier to use, and generates plots that look a whole lot better.  I wrote a [blog post](http://practicalcheminformatics.blogspot.com/2020/10/a-collection-of-things-i-freqently.html) that shows some of my favorite tricks with Seaborn. 


**Machine Learning Libraries**

[SciKit Learn](https://scikit-learn.org/stable/) - This is the ultimate machine learning library, which has the ability to perform many different unsupervised (clustering, dimensionality reduction, etc) and supervised (random forest, SVM, KNN) machine learning methods. It also includes many methods for data processing and model validation. 

[DeepChem](https://deepchem.io/) - Programming is like playing the piano, you don't learn it by reading books, you learn it by getting in there and doing it.  Probably the best way of learning to do machine learning for drug discovery is to mess around with the DeepChem codebase.  Bharath Ramsundar and Peter Eastman have implemented a host of useful methods and integrated a multitude of datasets.

[ChemProp](https://github.com/chemprop/chemprop) - Recent papers have demonstrated the utility of message passing neural networks (MPNNs) for QSAR.  One of the best implementations of this method is in the ChemProp package from MIT. 

[Faiss](https://github.com/facebookresearch/faiss) - As I've pointed out in a couple of [blog](http://practicalcheminformatics.blogspot.com/2019/01/k-means-clustering.html) [posts](http://practicalcheminformatics.blogspot.com/2019/04/clustering-21-million-compounds-for-5.html), K-means clustering and KNN can be useful methods in Cheminformatics.  The Faiss library from Facebook Research provides a fast, efficient method of performing these calculations.

[Minisom](https://github.com/JustGlowing/minisom) - Self organizing maps (SOMs) provide an easy means of grouping sets of related compounds.  Minisom provides an easy to use implementation thats good for datasets containing up to a few thousand molecules.  For bigger sets, try [Somoclu](https://github.com/peterwittek/somoclu).  I wrote a couple of blog posts about SOMS [here](http://practicalcheminformatics.blogspot.com/2018/10/self-organizing-maps-90s-fad-or-useful.html) and [here](http://practicalcheminformatics.blogspot.com/2018/10/self-organizing-maps-code-part-2.html). 

[RAPIDS](https://rapids.ai/) - This library from Nvidia enables the simple application of a variety of data science and machine learning operations on GPUs.  It can provide a quick and easy way of speeding up your workflows.  I wrote a blog post on RAPIDS [here](http://practicalcheminformatics.blogspot.com/2020/06/wicked-fast-cheminformatics-with-nvidia.html). 


### Databases

[ChEMBL](https://www.ebi.ac.uk/chembl/) - If anyone deserves sainthood, it's John Overington for making the ChEMBL database what it is today.  ChEMBL contains almost 2 million  compounds and more than 16 million assays datapoints.  It provides a wealth of useful data and has become a standard for computational chemical biology.   

### Database Searching

[FPSim2](https://github.com/chembl/FPSim2) - this package, from the same group at the EBI that produces the ChEMBL database, provides a fast easy means of performing fingerprint similarity searches.  I wrote a blog post about FPSim2 [here](https://practicalcheminformatics.blogspot.com/2020/10/what-do-molecules-that-look-like-this.html). 
