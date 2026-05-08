# ISA 401 Final Project: College ROI & Marketing Curriculum Analysis

## Technical Presentation Recording Link
https://youtu.be/TxAqigkhh1k 

## Tableau Dashboard Link
https://public.tableau.com/app/profile/victoria.rhodes/viz/TheValueofaMarketingDegreeExploringOhioPublicUniversityROI/ROI?publish=yes 

## Team Members
Group 20
- Mia Weber
- Victoria Rhodes
- Helen Kreitzer

## Research Question
What predicts college ROI for Marketing majors at Ohio universities?

## Data Sources
1. US Department of Education College Scorecard API
2. CampusReel scraped marketing salary data
3. University Marketing curriculum pages analyzed with LLM structured extraction

## Repository Contents
- api_doe_data.csv
- scraped_campusreel_data.csv
- unstructured_curriculum.csv
- college_roi.csv
- isa401_finalproject_apidata.Rmd
- isa401_finalproject_scrapeddata.Rmd
- isa401_finalproject_unstructureddata.Rmd
- isa401_finalproject_mergeddata.Rmd
- isa401_finalproject_exploratoryanalysis.Rmd *(code)*
- isa401_finalproject_exploratoryanalysis.html *(html with visible graphs)*

## Methods
- API collection with httr/jsonlite
- HTML scraping with rvest
- Structured extraction using ellmer + OpenAI
- Dataset merging and validation in R

## Workflow
1. Collect university financial data from the College Scorecard API
2. Scrape marketing salary data from CampusReel
3. Extract curriculum information from university marketing program pages using LLM structured extraction
4. Merge datasets into a final analytical dataset
5. Conduct exploratory analysis and visualization in R

## Data Validation
Datasets were merged by university name and manually checked for consistency across:
- tuition values
- earnings values
- debt values
- average salary values
- curriculum extraction outputs

Wright State University was excluded from the curriculum extraction analysis because the course description content was dynamically loaded and could not be consistently extracted using the same extraction workflow applied to the other universities.

## Reproducibility
To reproduce this project:
1. Open the `.Rmd` files in RStudio
2. Install required packages
3. Knit the files in workflow order:
   - apidata *(US Department of Education College Scorecard API)*
   - scrapeddata *(CampusReel scraped marketing salary data)*
   - unstructureddata *(University Marketing curriculum pages analyzed with LLM structured extraction)*
   - mergeddata
   - exploratoryanalysis

## Final Output
The final merged dataset is:
`college_roi.csv`

