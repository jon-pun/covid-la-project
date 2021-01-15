# Students: Check Your COVID-19 Privilege

  As part of my [Medium opinion piece](https://medium.com/swlh/students-check-your-covid-19-privilege-5914008f99ac) on colleges' and universities' abilities to perform COVID-19 testing on their students through fall 2020, I wanted to include the data and basic code used in the Tableau displays I provided.
  
  As such, they are available in this repository, sorted by project (Los Angeles / NYC).
  
  I'll be honest here: I am not a data analyst, nor have I taken upper-division coursework on statistical significance and analysis yet. As a foray, this was more of a "proof-of-concept" than anything else. That being said, I'm always open to comments, feedback, and especially concerns! Feel free to reach out to me on GitHub for whatever you may have to say.

## Data Sourcing

  The piece mentions sourcing data from NYC DPH and LA County DPH: in order to do so, the daily files taken from each site's respective data repositories or websites (in CSV format) are attached under each location's respective folders. Dates of collection are listed as the titles, and are left "as found."
  
## Geocoding

  Although the NYC DPH data contains MODZCTA (modified Zip Code Tabulation Areas) that could be displayed in Tableau, LA County Data only included place or neighborhood names, and thus could not be automatically geocoded. As a result, some automatic geocoding was done with [geocod.io](https://www.geocod.io/upload/), and the rest (inaccurate placements, erroneous names, etc.) were manually corrected afterwards with Google Maps. 
  
## Data Manipulation

  In order to look between days, average multi-day periods together, and also find basic statistics in the data such as percent change, data was uploaded to and manipulated within Rstudio using the R programming language. The project files, as well as some R Markdown files, are included under each location's folders. 
  
## Tableau Workbooks

  To display "findings," I created Tableau workbooks containing manipulated data, added sheets to visualize the data, and had them hosted on Tableau Public. The workbooks themselves have been uploaded, one in each location's folder. To view the interactive visualizations themselves (regrettably, Medium does not allow HTML code to be inserted), check here for [LA](https://public.tableau.com/views/LA-County-Testing-Changes/TestingRateChanges?:language=en&:display_count=y&:origin=viz_share_link) and [NYC](https://public.tableau.com/views/ChangestoNYCsOverallNumberofTestsCompleted/COVIDTesting?:language=en&:display_count=y&:origin=viz_share_link). 
