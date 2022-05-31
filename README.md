> NOTE: For the revision I am starting this over so that the conservation actually works this time:)

# Artifact Description

The following are main directories of the artifact. The directories are usually accompanied by an extra readme with details about the items therein: 

- `artifact` contains the R notebooks and support functions required for the paper itself, not the reproductions
- `reproductions` contains R notebooks that reproduce the papers
- `paper` contains the paper itself.

The generated folders are:

- `figs` for figures used in the paper
- `latex-include` for the numbers and other stuff generated by the notebooks to be included in the paper's latex source

The linked folders (dataset) are:

- `dataset` which should be populated with the dataset as described in the section below

> Note that not all parts of the dataset folder are required to run the artifact. 

## Reproductions

### What Constitutes the Software

Consists of a single R notebook that analyzes the composition of projects.   

# Datasets

All data to the artifact should be located on `prl-parasite` in `/mnt/data/codedj-2-artifact` using the following structure:

- `dataset/java` contains the merged Java dataset
- `dataset/python` contains the merged Python dataset (note that this also contains a lot of C/C++ projects)
- `dataset/js` contains the merged JavaScript dataset
- `djanco-cache/java` contains djanco cache for Java (NOTE: not sure this is valid)
- `djanco-cache/python` contains djanco cache for Python
- `djanco-cache/js` contains djanco cache for JavaScript
- `reproductions` contains results for the papers we reproduce. See their details below. 

## Reproduction Datasets

Contains information about the reproductions. At least following is necessary for each, here given as example for the _What constitutes a software_ paper:

- `reproductions/what-constitutes-software/query` is the git repository with djanco queries producing the selections required for the reproduction
- `reproductions/what-constitutes-software/results` contains the results obtained by the query above

For more details see the respective R notebooks of the reproduced papers. 




# OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD

# TODO To deanonymize

CHECK AND REMOVE THIS BEFORE ANONYMIZING

- check for our names in files and remove
- remove our names from the paper (!!!)
- check prl-prg in names and files and verify that it's ok
- replace the dataset getters to get them from the anonymized repo release

# The Fault in Our Stars

> This is the anonymized state of our artifact right after the paper submission. Everything should work, but there might be rough edges. A deanonymized, cleaned and polished version of this document will be published for the artifact evaluation if our paper is accepted. Everything in here *should* work, but the anonymization might have broken things here or there and rerunning the entire artifact from scratch takes a *lot* of time so not all errors might be fixed immediately.  

## Artifact contents

A brief description of the folders in the artifact follows:

- `artifact` contains the R scripts and tools used for the figures and numbers reported in the paper *unless* they are in the other folders decribed below
- `dataset` contains the smaller datasets required for the reproductions. The big datasets are too big to be part of the artifact on github and are discussed below
- `figs` contains the figures gerenated for the paper
- `latex-include` contains the generated special commands that add numbers to the paper
- `msr-meta` contains detailed information about the metaanalysis of the MSR papers from 2019 and 2020 that is part of our paper
- `paper` contains the actual paper
- `reproductions` contains the reproductions of the four papers that appear in our paper and create the graphs and numbers generated by those

## Datasets

We used the CodeDJ datasets available at the time. These are archived on our server in `/mnt/data/icse2021` in both raw and merged forms. Here is a quick description:

- `java-raw` = the raw Java datasets. Obtained from GHTorrent, only non-forked Java projects. 
- `python-raw` = the python raw dataset. Obtained from GhTotrrent, contains C++ and Python projects. 
- `js-raw` = the javascript raw dataset. Obtained from GHTorrent, contains JavaScript and some Python (Python projects from this dataset were not used in the paper)
- `java-merged` = Java merged datastore, all substores from `java-raw` merged into generic
- `python-merged` = Python merged datastore, all substores from `python-raw` merged into generic
- `js-merged` = JavaScript merged datastore, JavaScript and small projects substores from `js-raw` merged into generic

## Running

The artifact is organized into various R notebooks. These are best executed from the RStudio. Note that all notebooks opened in RStudio share the same environment. After installing RStudio set the current working directory to the root of the artifact (the directory containing this readme file) and execute in the following order:

1. `artifact/dataset.Rmd` - this loads up our datasets and produces figures and numbers describing them as well as the basic selections analyzed
2. `artifact/stars-analysis.Rmd` - the manual analysis of the top starred projects. No need to run this, as all the analysis done was manual. 
3. `msr-meta/msr.Rmd` - the manual metaanalysis of MSR papers. No need to run, it only creates graphs and figures we used to describe the papers' use of sampling
4. `reproductions/what-constitutes-software/what-constitutes-software.Rmd` to reproduce *What is Software*
5. `reproductions/empirical_method_chaning/reproduction.Rmd` to reproduce *Method Chaining*
6. `reproductions/style_analyzer/style_analyzer.Rmd` to reproduce *Style Analyzer*
7. `reproductions/scent-dl/scent_dl.Rmd` to reproduce *Code Smells*
8. build the paper, enter the `paper` folder and run `make`. `main.pdf` will be created producing the paper. 

## Notes

Due to limited access to CodeDJ a the sizes of the datasets and nature of our work allowing local processing to certain degree we have ran CodeDJ queries that summarized all the projects in the datasets into csv files and then used Rstudio to report & replay selections locally for faster turnaround. These CSVs are part of the `dataset` folder in the artifact. We do have CodeDJ queries for all queries executed, but can't share their receipts as these would immediately give away our identities. These will be part of the deanonymized artifact if accepted. 

Additional datasets are loaded by the reproductions. List of all datasets that are small enough to be part of the repo can be found in the Github releases of the artifact. 

The repository contains all the files produced as well, i.e. you can skip the steps above and proceed directly to producing the paper, or cherry pick those you are interested in. Note, however, that the `artifact/dataset.Rmd` file populates the R environment required by the other Rmds and therefore must be loaded if other R files are. 




