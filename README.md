# An Investigation of Political Partisanship Across Time using Data Science

By Vlad Dobrin and James Biggins

## View our Project Here
https://jabiggins.github.io/PoliticalPartisanshipInCongress.html

## Reproducibility

Our project is long, and has a lot of moving parts. If you are simply looking at the project, then ignore this section. If want to reproduce it, keep reading.

#### Environment:
We did development in Google Colab, I reccommend that you do the same or else you are going to have to modify the code a little.

#### Time Sensitivity
Web scraping the data took two weeks to fine tune, and even if you don't make any mistakes it will take a couple days of pure runtime to get all the information. As you will read, I gave detailed information on how to scrape a subset of the total data we use for this project, called a **batch**. I reccommend that you play around with the example I provided if you want to test that our scraping code works. This way, you don't have to waste days waiting for the entire scrape to finish.

#### Important files
Assuming you have convinced yourself that our scrape works, we included 4 files that you will need to upload to the Google Colab project in order to get to all the ML stuff. 
* houseCongressTable
* houseVoteTable
* senateCongressTable
* senateVoteTable

These files contain the entirety of the scraped and cleaned data that will be used in sections 3 and 4. Once you uploaded everything, start execution at the big bold checkpoint section on the table of contents, you can't miss it.

## Table of contents



1.   Part 1: Data Collection
>*   Identify a raw data source
>*   Scrape the data

2. Part 2: Data Processing
>* Part 2a: Data Pre-processing
>>* Convert the individual arrays of information into two pandas dataframes
>>* Clean the scraped data
>>* Batch Download
>* Part 2b: Data Post-processing
>>* Batch Uploads
>>* Delete attribute that gets added during csv conversion
>>* Batch Stitching
>>* Final Cleaning
>>* Final Cleaning
>>* Final Post-Processing

**Checkpoint: Use our data to avoid the scraping steps above**

3. Part 3: Exploratory Analysis & Data Visualization
>* Senate Representation and PercentYea Analysis
>* Partisanship in Congress
>>* Partisanship in the Senate
>>* Partisanship in the House
4. Part 4: Analysis, Hypothesis Testing and Machine Learning
>* The Necessity of Averaging
>* Senate: Multilinear Linear Regression
>* House: Multilinear Linear Regression
>* Senate Ridge Regression
>* House Ridge Regression
>* Senate Nearest Neighbor
>* House Nearest Neighbor
5. Part 5: Insight, Policy Decision, and Importance
>* Summary
>* Financial Importance
>* Social Importance
>* The future of this project
