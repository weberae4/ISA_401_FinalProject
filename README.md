# ISA 401 Final Project: College ROI & Marketing Curriculum Analysis

## Research Question
What predicts college ROI for Marketing majors at Ohio universities?

## Team Members
- Mia Weber
- Victoria Rhodes
- Helen Kreitzer

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

## Methods
- API collection with httr/jsonlite
- HTML scraping with rvest
- Structured extraction using ellmer + OpenAI
- Dataset merging and validation in R

## Final Output
The final merged dataset is:
`college_roi.csv`
