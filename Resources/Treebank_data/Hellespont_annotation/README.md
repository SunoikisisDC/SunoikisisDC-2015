#Hellespont materials
##What is this?
This folder includes all the treebank files and resources produced during the [Hellespont Project](http://hellespont.dainst.org/startpage/). In particular, it provides all the materials that should be needed in order to visualize, browse, query and manipulate our flagship **Tectogrammatical Annotation** of Ancient Greek. Yuhuuuu!

If you want to know more about Tectogrammatical Annotation of Greek, please refer to the [Documentation](http://hellespont.dainst.org/startpage/docu.html#Linguistic-Annotation) of Hellespont and the literature quoted there, or you may want to read this tiny little [blog post](http://wp.chs.harvard.edu/chs-fellows/2013/03/08/deep-into-the-meaning-tectogrammatical-annotation-of-ancient-greek/) of mine. Don't be scared, it's a lot of fun!

##What files do we have?
The actual treebanks files are provided in two different (yet slightly equivalent) formats:

1. the **Treex** format (in the treex folder), which includes a bunch of supplementary information on the named entities and is visualized with the two trees for the sentences side by side

2. the 3-layer format typical of the **PDT 2.0** (Prague Dependency Treebank), where the information is stored in 4 different files: text (.w), morphology (.m), surface syntax, or analytical (.a), tectogrammatical (.t)

The rest of the folder includes a few supplementary resources:

* the xml schemata for the annotation of Greek; note: you will **need them** if you want to work with the annotation (see next question)

* the valency dictionary: strictly speaking, you won't need it, but it's a fundamental part of the linguistic annotation.
	
##What should I do with all this?

You can easily open, visualize, query and even edit the files with the software [TrEd](http://ufal.mff.cuni.cz/tred/), developed by the team of the Prague Dependency Treebank:

1. go to the [TrEd page](http://ufal.mff.cuni.cz/tred/)

2. follow the instructions for your OS; note that:

* if you're on **Linux**: TrEd will install very easily; the only complication that you may find is that some Perl libraries are missing. Read the installation log and install all the required packages.

* if you're on **Mac**: the .dmg file is also installed very easily; I honestly don't remember if they are required by the latest version, but it's always a good idea to have the Xcode utilities installed (some add-ons require them) Unfortunately, though, I have experienced an annoying bug on Yosemite that makes it almost impossible to use the GUI...

3. open TrEd and install a bunch of useful plugins. I would recommend:

* **PML-Tree Query** (see next question)
* **Easy Treex**, that will let you see the .treex files

**IMPORTANT**: in order to load the files, TrEd must be able to find the appropriate schemata. The easiest thing is simply to copy the whole content of the "schemata" subfolder in the same folder where you are keeping the annotation files.

##What about querying?

TrEd includes a hyper-cool plugin for querying the treebanks called [PML-TreeQuery](http://ufal.mff.cuni.cz/pmltq/doc/pmltq_doc.html). You can easily install PML-TQ from the Add-on menu of TrEd.

Unfortunately, PML-TQ doesn't seem to work (at least in my experience) with .treex files, so you will have to use the PDT 2.0 format to do your research. But with them, it will work like a charm!

If you know something about Perl and/or you feel particularly brave you two options:

1. use a command line tool called [Btred](http://ufal.mff.cuni.cz/pdt2.0/doc/tools/tred/bn-tutorial.html) (which is installed together with TrEd)

2. install [Treex](http://ufal.mff.cuni.cz/treex) and write your own scenarios (on Unix)

##Ok, I feel brave: I want to install Treex!

Then, follow [these instructions](http://ufal.mff.cuni.cz/treex/install.html) and have fun. Good luck!

(just kidding, it is actually not difficult at all and the instructions are very detailed and well written.)

Once you've done, don't forget to familiarize with Treex with this nice [tutorial](http://ufal.mff.cuni.cz/treex/firststeps.html).