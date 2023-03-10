# Beer Advocate Beer Review Analysis

## Project Notes
- Our data source file is over 200MB. Over 30MB when zipped. We attempted lfs and were not successful. Please see this link for our data.
https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate
- We chose to use the initial csv (after cleaning) as our database. We created a mockup ERD only.

![image](https://user-images.githubusercontent.com/109913335/215339585-e62f7652-5e49-4eec-9cae-e385efc0659b.png)


## Group Assignments & Communication Protocols
### Assignments
 - Brad: clean, data insights, python, google slides collaboration
 - Noa: tableau visualizations, data insights, google slides collaboration
 - Sanjay: data cleaning, machine learning model and reasoning, database erd, google slides collaboraton
 - Emily: data cleaning, machine learning model and reasoning, data cleanng, project manager, google slides collaboration
 
 ### Communication Protocols
  - Established a slack channel for communication
  - Met during class time and Sundays. Worked individually in between group meetings.

## Outline/Storyboard
 - Topic and Reasoning
 - Data Source
 - What can the data tell us?
 - Data Exploration Process
 - Dataset at a Glance
 - Analysis Phase
 - Results - Models
 - Dashboard Analysis and Results
 - Technologies, Languages, Tools, and Algorithms
 - Recommendations for a Future Analysis
 - Reflection

## Link to Google Slides presentation

https://docs.google.com/presentation/d/16uvX4NDOVZA92_KLJNtno265sSpNJKDcykty3R15uHI/edit?usp=sharing

## Database
      - https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate

## Content
The presentation tells a cohesive story about their project, including the following:

**Selected topic:** 
      
      - Beer Advocate Beer Reviews

**Reason for selecting the topic**

     - Digestible topic
     - Beer is universal
     - Applicable to demographic of the project audience
     - Cheers

**Description of their source of data** 

     - Beer Reviews from Beer Advocate
     - https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate
     - Large data set (1.5 million reviews)
![image](https://user-images.githubusercontent.com/109913335/215336653-e934b8aa-1a6a-42e1-bf4c-a7adfbd7681e.png)
    
**Questions to answer with the data**

     - What beer style gets the best overall review scores?
     - Which feature contributes the most to an overall review score over 3?
     - Show the all the features and their associated importance.
     - Show the features that contribute the most and least to the overall review score, and how they relate to the overall review score. 
     - Show the breweries and average overall review. Allow the user to select a set of breweries and/or an overall review range.
     - Show the average overall review by ABV. Allow the user to select an ABV range and/or beer style.


**Description of the data exploration phase of the project**

    - Opened the CSV in excel and scanned data to get the feel of it
    - Imported Dependencies and Read beer_reviews.csv into a dataframe
    - Displayed the first 5 rows of the dataframe
    - Looked for null values
    - Displayed the number of unique values for each column
    - Displayed the data types
    - Displayed the value counts of several columns

**Model analysis and results**

      - See Google Slides (https://docs.google.com/presentation/d/16uvX4NDOVZA92_KLJNtno265sSpNJKDcykty3R15uHI/edit?usp=sharing)
      - Preprocessing including removing null values, identifying the features and target variables, removing non-beneficial columns, converted our target values to 0 and 1 so we could create a classification machine learning model.
      - Our data is imbalanced with only 17% from the minority class, so we resampled using SMOTEENN.
      
![image](https://user-images.githubusercontent.com/109913335/217132207-89e53a22-736b-458f-b22b-caf02aab78e1.png)
  
      - Started with Logistic regression
      
![image](https://user-images.githubusercontent.com/109913335/217132283-9d10e678-99e5-4cc8-b3b4-f9b470e29b3d.png)

      - Created a confusion matrix.
      
![image](https://user-images.githubusercontent.com/109913335/217131019-323aec12-1be8-4ed6-99df-a5020de52426.png)
    
      - Logistic Regression Results

![image](https://user-images.githubusercontent.com/109913335/217130951-3eab30f4-acfe-48c8-8d91-463c21c8b212.png)

         - Overall Accuracy = 86.%
         - Good precision for positively predicting which beers will have a review over 3. Less precision for predicting beers with an overall review score of 3 or under. 
         - Good recall for both overall review buckets.
         - Good F1 scores, but better for beers with an overall review over 3
       - Tried to get a better result with Random Forest
     
![image](https://user-images.githubusercontent.com/109913335/217131473-882104d2-a5c0-46c1-9ab0-4cab6fc49ac1.png)

         - Created a confusion matrix
         
![image](https://user-images.githubusercontent.com/109913335/217131674-750dc123-e4a0-4eca-a265-891d83a8ac20.png)

         - Random Forest Results
         
![image](https://user-images.githubusercontent.com/109913335/217131806-b666e4fd-8252-4355-a4d2-cdca449eaf76.png)

           - Overall Accuracy = 90.6.%
           - Good precision for positively predicting which beers will have a review over 3. Less precision for predicting beers with an overall review score of 3 or under. 
           - Recall suffers a bit for for beers with an overall review score of 3.
           - Logistic regression produced a similar recall score prior to resampling.
           - Good F1 scores, but better for beers with an overall review over 3 
         

**Technologies, languages, tools, and algorithms used throughout the project**

      - Microsoft Excel
      - Jupyter Notebook
      - Tableau
      - Github
      - Google Slides
      - Python
      - Machine learning

**Recommendation for future analysis**

       - Adjust bucketing to overall reviews of 4 and over, and under 4.
       - Capturing the number of beers/alcoholic drinks the beer reviewer has consumed prior to each review - Does the overall review score improve with the number of beers consumed? 
       - Capturing location data for the breweries to put together ultimate beer tours based on a user???s beer style preference and overall review scores.
       - Capturing more data on if any breweries distill their own liquor or ferment their own wine in addition to brewing their own beer - to what extent does a brewery that makes more than just beer have higher or lower reviews?


**Anything the team would have done differently**

       - Spent more time ideating the topic and potential scope of project
       - Research ways to improve the recall score on the positive predictions of the Random Forest Model

### Machine Learning Model
Team members present a provisional machine learning model that stands in for the final machine learning model and accomplishes the following:

**Takes in data in from the provisional database**

      - beer_reviews.csv
      
**Outputs label(s) for input data**
 - Features = all have the same scale of values from 0 to 5, except beer_abv. All are numeric.
    - review_aroma
    - review_appearance
    - review_palate
    - review_taste
    - beer_abv
 - Target variable = review_overall (3 or under, or 3.5 or higher)

**Working code on main branch under Logistic Regression and Random Forest Models**

    - See attached Logistic Regression and Random Forest Jupyter Notebooks
    - See Google slide deck for the below 1-7 deliverables
1. Description of data preprocessing 
2. Description of feature engineering and the feature selection, including the team's decision-making process 
3. Description of how data was split into training and testing sets 
4. Explanation of model choice, including limitations and benefits 
5. Explanation of changes in model choice (if changes occurred between the Segment 2 and Segment 3 deliverables) 
6. Description of how model was trained (or retrained, if they are using an existing model) 
7. Description and explanation of model???s confusion matrix, including final accuracy score

Note: If statistical analysis is not included as part of the current analysis, include a description of how it would be included in the next phases of the project.


## Dashboard

**Storyboard on Google Slide(s)**

**Description of the tool(s) that will be used to create final dashboard**

      - Tableau Desktop
      
**Description of interactive element(s)**

      - Show the breweries and average overall review. Allow the user to select a set of breweries and/or an overall review range.
      - Show the average overall review by ABV. Allow the user to select an ABV range and/or beer style.




Working Notes
- Data at a glance: overview tab to give the user a good idea of how much data, what kind of data, etc they are seeing
- Brewery tab: ability to check one or multiple breweries and toggle a review slider to see  reviews by brewery, beer type and reviewer
- Beer tab: ability to check one or more beer types and toggle a review slider to see overall reviews, reviews by taste, aroma, flavor, etc.
- ABV tab: ability to check one or more ABV level and a toggle a review slider to see overall reviews, reviews by brewery and review by taste
