# Overview

This repository contains the code and products created for the project on HPV vaccination completion rates depending on several socioeconomic factors, by Kelly Cao and Rachel Robertson.

# Purpose

This project performs exploratory and statistical analysis to determine which geographic and socioeconomic factors play the largest role in HPV completion rates among U.S. teens. The data is gathered from the 2022 NIS Teen Vaccination surveys, which are administered to the parent or guardian of a teenager along with the provider to gather demographic information on the teen in tandem with their vaccination history. The socioeconomic and demographic predictors of HPV vaccination rates that are examined include: Race/ethnicity, state of residence, geographic mobility, income, poverty level, housing status, maternal education, insurance status, language, and facility in which the survey was administered. 

# Pre-requisites

This data analysis project uses R, Quarto, Github and a Zotero. It is also assumed that you have a word processor installed (e.g. MS Word or [LibreOffice](https://www.libreoffice.org/)). You need that software stack to make use of this template.

# Structure

* All data goes into the subfolders inside the `data` folder.
* All code goes into the `code` folder or subfolders.
* All results (figures, tables, computed values) go into `results` folder or subfolders.
* All products (manuscripts, supplement, presentation slides, web apps, etc.) go into `products` subfolders.
* The `renv` folder is automatically generated by the `renv` package, and is
used to keep track of packages.
* See the various `README.md` files in those folders for some more information.

# Getting Started

You may first copy this template using the link to our Github [insert link here]. After copying the repository, you may run the code in this order:

* In the 'code' folder, select the 'processing-code' subfolder
  * First, under the 'processing-code' subfolder, you may choose to render     'Processing-Quarto-Output.qmd' to view the code in chunks with commentary
* Return to the main 'code' folder and select the 'eda-code' subfolder
  * Run and render 'EDA-code.qmd' to view the code chunks with commentary
* Return to the main 'code' folder and select the 'analysis-code' subfolder
  * First, run and render 'analysis1.qmd'
  * Next, run and render 'analysis2.qmd'
[more code files to be added to analysis code]

 <hr>
** To view the manuscript **

* In the `products` directory, enter the `manuscript` folder. 
  * The manuscript can be viewed either by downloading and viewing  `Manuscript.docx` or opening and     rendering `Manuscript.qmd`. Either ways will allow you to view a word document of the manuscript. 


# Findings

[Insert final predictors found to greatest impact HPV completion rates here]

# Dr.Handel's notes [ignore if reviewing project]:
## Template content 

See the `readme` files in each folder for more details.

* There is a simple, made-up dataset in the `raw_data` folder. 
* The `processing_code` folder contains several files that load the raw data, perform a bit of cleaning, and save the result in the `processed_data` folder. 
* The `analysis_code` folder contains several files that load the processed data, do an exploratory analysis, and fit a simple model. These files produce figures and some numeric output (tables), which are saved to the `results` folder.
* The `results` folder contains code output, includeing figures, tables saved as serialized R data (`.Rds`) files, and other outputs (distinct from data because they are generated by code).
* The `assets` folder contains static assets like pre-generated schematics from BioRender, bibtex files, csl files, and PDFs of references. These assets are not code-based and are not generated by code.
* The `products` folder contains final deliverables, like slides, the manuscript, the supplement, and posters.
  * The  `manuscript` folder contains a template for a report written as Quarto file. If you access this repository as part of [my Modern Applied Data Science course](https://andreashandel.github.io/MADAcourse/), the sections are guides for your project. If you found your way to this repository outside the course, you might only be interested in seeing how the file pulls in results and references and generates a word document as output, without paying attention to the detailed structure. There is also a sub-folder containing an example template for a supplementary material file.
  * The `slides` folder contains a basic example of slides made with Quarto.
* The `renv` folder is automatically generated by the `renv` package and you
should never edit it manually. This folder is used to store information about
the packages you are using in your project.
* There are multiple special files in the repo.
  * `README.md`: this file contains instructions or details about the folder it
  is located in. You are reading the project-level `README.md` file right now.
  * `renv.lock`: a special file in JSON format used to keep a log of which
  packages and versions your project uses.
  * `.gitignore`: this file gives instructions to the version control system,
  Git, and tells it which files we do not need to record versions of. Usually
  these are various files containing local settings.
  * `.Rprofile`: whenever you restart the R session, R will source (run all
  code in) this script. Right now this is used by `renv` to make sure we have
  the correct packages and versions installed.


# Getting started

This is a Github template repository. The best way to get it and start using it is [by following these steps.](https://help.github.com/en/articles/creating-a-repository-from-a-template)

Once you got the repository, you can check out the examples by executing them in order. First run the processing code, which will produce the processed data. Then run the analysis scripts, which will take the processed data and produce some results. Then you can run the manuscript, poster and slides example files in any order. Those files pull in the generated results and display them. These files also pull in references from the `bibtex` file and format them according to the CSL style.

You can read about keeping track of projects with `renv`
[here](https://rstudio.github.io/renv/articles/renv.html).
Basically, whenever you install new packages or update old packages, you need
to run `renv::snapshot()` to update the `renv.lock` file, which is a list of
packages and versions that the package uses. When you open the R project on a
new computer, you can run `renv::restore()` to reinstall all the packages that
you recorded in the `renv.lock` file.


