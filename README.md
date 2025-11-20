# Visualize Social Patterns with the Census API

_Author_: John Lauermann, School of Information, Pratt Institute

This repository contains materials for a workshop with the [Data Storytelling Lab](https://github.com/DataStorytellingLab) at Pratt Institute. The workshop covers how to query data from the Census API and then visualize and analyze it using R tools. 

In this workshop, you’ll learn how to visualize and analyze data from the US Census. Census data products are the primary historic record of American society, available as open data for every community in the United States. The long temporal record and diverse geographic scope of these data present opportunities for data storytelling at scale. Census data allow you to tell stories that move beyond small scale case studies, to think about national patterns and historic trends. 
To work with this kind of big data, we’ll use open source statistical tools in R to analyze and visualize geographic patterns. 
<br>

## Learning outcomes
By the end of the workshop, you should be able to: 
1)	Query American Community Survey data from the Census API. 
2)	Visualize patterns in the data using choropleth maps and scatterplots.
3)	Analyze whether those patterns are statistically significant using correlation and simple linear regression. 

## How to set up
Initial set up steps include:
- Sign up for a Census API key at [this link](https://api.census.gov/data/key_signup.html)
- Install R and RStudio on your computer with [this link](https://posit.co/download/rstudio-desktop/)
- Download the code version of this workflow: [`visualize-social-patterns-census-api.rmd`](visualize-social-patterns-census-api.Rmd). (go to the page, click the download button on the top right)
- Open the `.rmd` notebook in RStudio (from the top left menu bar: File -> Open File)

You can replicate the workflow step by step using the code chunks in the notebook. To run each chunk, either click the green ‘Run Current Chunk’ button or put your cursor in the code block and hit either `Cntrl + Shift + Enter` (for a PC) or `Cmd + Shift + Enter` (for a Mac). 

To see the full scope of the this workshop, you can check out the markdown version of the notebook: [`visualize-social-patterns-census-api.md`](visualize-social-patterns-census-api.md).
<br>

## Basic workflow
1)	Install and load the libraries we’ll need for the workflow. 
2)	Explore Census data and define a query to pull two variables from the API for further analysis. For this we’ll use `tidycensus` to query the Census API and `dplyr` to clean up the data table.
3)	Visualize the geographic distribution of each variable using choropleth maps built with `ggplot2`.
4)	Visualize the relationship between those two variables using a scatterplot built with `ggplot2`. 
5)	Test the correlation between those variables using `cor.test()`
6)	Test whether one variable predicts the other using simple linear regression with the `lm()` function.

## Further reading
- Walker, Kyle (2023) _Analyzing US Census Data: Methods, Maps, and Models in R_, CRC Press (open access at https://walker-data.com/census-r/)
- Wickham, Hadley (2025) _ggplot2: Elegant Graphics for Data Analysis_, Springer (open access at https://ggplot2-book.org/preface-3e.html)
<br>
<br>
<br>

Shield: [![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This work is licensed under a
[Creative Commons Attribution-NonCommercial 4.0 International License][cc-by-nc].

[![CC BY-NC 4.0][cc-by-nc-image]][cc-by-nc]

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-image]: https://licensebuttons.net/l/by-nc/4.0/88x31.png
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg
