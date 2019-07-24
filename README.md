## INSTALLATION ##

Step 1. 
Install R and R Studio by following the prompts at the following websites

Recommended to use an older version of R (say December 2018) as some R packages are not compliant with newer versions of R: https://cran.r-project.org/bin/windows/base/old/

- Windows - https://cran.r-project.org/bin/windows/base/
- Mac - https://cran.r-project.org/bin/macosx/
- R studio - https://www.rstudio.com/products/rstudio/download/

Step 2.
Install latest version of Python by following the prompts at the website below

https://www.python.org/downloads/ - Choose the prompts based on the operating system you are using. 

Step 3.
Open R Studio and copy/paste (or type) in the following command into the R Studio console window:

install.packages("shiny", "shinyFiles", "DT", "tcR", "shinyjs", "dplyr", "ggplot2", "reticulate")

Step 4. Download Immunarch package by going to the website: https://immunarch.com/articles/1_introduction.html

After downloading the Immunarch.tar.gz file then run the following two commands in the R Studio console window (replacing "path/to/your/folder/with/immunarch.tar.gz" with a path to the folder that contains your immunarch.tar.gz) :

install.packages("devtools", dependencies = T)

and:

devtools::install_local("path/to/your/folder/with/immunarch.tar.gz", dependencies=T)

## RUNNING APP ##
 
Step 1. 
Download the CoEve Shiny app by using the Github “Clone or Download” button on this page. Then make sure that you have the following files (preferably saved in the same folder):

- Metadata (please call this metadata.txt)
- Mixcr files to analyse
- "shinyApp" folder containing the app.R file

Step 2.
Open app.R in R Studio and click Session > Set Working Directory and choose the directory which the "shinyApp" folder is contained

Step 3. 
Click "Run App" button and if all packages have installed properly, a new window should open up with the app

Step 4.
Follow the navbar options from left to right on the app 
NOTE: Mixcr file names should be kept to 13 characters or less otherwise one of the graphs produces an error