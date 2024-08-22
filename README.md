# Web Scraping and Data Management in R <img src="https://media.giphy.com/media/1oGT95WukVFcRO1OFZ/giphy.gif" width="50">

[![](https://img.shields.io/badge/Language-R-blue)](http://cran.r-project.org/)

<sub>*Last updated 2024-03-21.*</sub>

This GitHub repository includes R code for web scraping, data wrangling, and reporting, developed as part of my exam for the Web Scraping and Data Management module in the MA Social Science Data Analytics course. The project involves scraping tables from four Wikipedia web pages, processing the data, and creating a SQLite database for storage and analysis. Additionally, the repository demonstrates how to set up and execute SQL queries from R to combine data from multiple tables. The analysis focuses on evaluating whether high nominal GDP per capita correlates with better quality democracy. Data is sourced from the following Wikipedia pages:

[List of countries by GDP (nominal) per capita](https://en.wikipedia.org/wiki/List_of_countries_by_GDP_(nominal)_per_capita)

[Democracy indices (V-Dem)](https://en.wikipedia.org/w/index.php?title=V-Dem_Democracy_Indices&oldid=1233003638)

[The Economist Democracy Index](https://en.wikipedia.org/w/index.php?title=The_Economist_Democracy_Index&oldid=1229762903)

[Bertelsmann Transformation Index](https://en.wikipedia.org/w/index.php?title=Bertelsmann_Transformation_Index&oldid=1219713517)

**Web Scraping and Data Management using [`rvest`](https://cran.r-project.org/web/packages/rvest/index.html)**. 
## :telescope: Overview

The repository is organised into the following sections:

- **[1.0 User Guide](/1.0_User_Guide))**: This is a procedure guide for using the `rvest` package for web scraping, `tidyverse`, `stringr` and `purrr` for some data wrangling and xml2 for parsing HTML data, as well as `DBI` for interacting with relational databases in R, `RSQLite` for implementing the `DBI` interface specifically with SQLite databases and `ggplot2` for data visualisation
- **[2.0 Instruction Sheet](/2.0_Instruction_Sheet)**: This is the instruction sheet for the exam that details what to web scrap and report.
- **[3.0 Data File](3.0_Data_File)**: This is the.csv output file to review course information at the Essex Summer School including the course names, URLs and descriptions.

## :scroll: Notes

This repository assumes basic competence in R (setting working directory, loading packages, etc) and contains only materials relating to *Web Scraping and Data Management in R*. So the focus will be generally on the application and not on the theory.  

## :hammer_and_wrench: Setup

To run the code, you will need:

1. A fresh installation of [**`R`**](https://cran.r-project.org/) (preferably version 4.4.1 or above).
4. [RStudio IDE](https://www.rstudio.com/products/rstudio/download/) (optional but recommended).
5. Install the required packages by running:

   ```R
   # Load the package
   pacman::p_load(rvest, tidyverse, stringr, purrr, xml2, DBI, RSQLite, ggplot2)
   ```

<details>
<summary>
<i>Package Versions</i>
</summary>
   
Run on Windows 11 x64 (build 22621), with R version 4.3.2.

The packages used here:

- `revtools` 	1.0.4(*CRAN*)
- `tidyverse` 2.0.0(*CRAN*)
- `stringr`   1.5.1(*CRAN*)
- `purrr`     1.0.2(*CRAN*)
- `xml2`      1.3.6(*CRAN*)
- `DBI`       1.2.3(*CRAN*)
- `RSQlite`   2.3.7(*CRAN*)
- `ggplot2`   3.5.1(*CRAN*)
- `pacman`    0.5.1(*CRAN*)
</details>

Feel free to adjust this based on your preferences and specific details about your code and setup.
