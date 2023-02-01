# Beer Advocate Beer Review Analysis

## Sections in general
- Presentation:
  - Google Slides
- GitHub:
  - Branching, commits
  - The descriptions and explanations required in all other project deliverables should also be in your README.md as part of your outline, unless otherwise noted.
- Machine Learning Model:
  - Working model
  - Full description of steps with explanations
  - Answers the question
- Database
   - Integrated database
   - At least 2 tables, 1 join, 1 connection string
- Dashboard
  - Data story that is logical and easy to follow
  - Images from the initial analysis
  - Data from the machine learning task
  - At least one interactive element

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

## Overall Rubric deliverables (bolded as completed)
### Presentation
#### Content
The presentation tells a cohesive story about their project, including the following:

**1. Selected topic:** 
      
      - Beer Advocate Beer Reviews

**2. Reason for selecting the topic**

     - Digestible topic
     - Beer is universal
     - Applicable to demographic of the project audience
     - Cheers

**3. Description of their source of data** 

     - Beer Reviews from Beer Advocate
     - https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate
     - Large data set (1.5 million reviews)
![image](https://user-images.githubusercontent.com/109913335/215336653-e934b8aa-1a6a-42e1-bf4c-a7adfbd7681e.png)
    
**4. Questions to answer with the data**

     - What beer style gets the best overall review scores?
     - Which feature contributes the most to an overall review score over 3?
     - Show the all the features and their associated importance.
     - Show the features that contribute the most and least to the overall review score, and how they relate to the overall review score. 
     - Show the breweries and average overall review. Allow the user to select a set of breweries and/or an overall review range.
     - Show the average overall review by ABV. Allow the user to select an ABV range and/or beer style.


**5. Description of the data exploration phase of the project**

    - Opened the CSV in excel and scanned data to get the feel of it
    - Imported Dependencies and Read beer_reviews.csv into a dataframe
    - Displayed the first 5 rows of the dataframe
    - Looked for null values
    - Displayed the number of unique values for each column
    - Displayed the data types
    - Displayed the value counts of several columns

**7. Description of the analysis phase of the project**

      - See Google Slides (https://docs.google.com/presentation/d/16uvX4NDOVZA92_KLJNtno265sSpNJKDcykty3R15uHI/edit?usp=sharing)

**8. Technologies, languages, tools, and algorithms used throughout the project**

      - Microsoft Excel
      - Jupyter Notebook
      - Tableau
      - Github
      - Google Slides
      - Python
      - Machine learning

**9. Result of analysis** 

      - see Model notebook3.ipynb on main branch, and Google Slides

**11. Recommendation for future analysis**

       - Capturing the number of beers/alcoholic drinks the beer reviewer has consumed prior to each review - Does the overall review score improve with the number of beers consumed?
       - Capturing location data for the breweries to put together ultimate beer tours based on a user’s beer style preference and overall review scores.

**12. Anything the team would have done differently**

       - Random Forest with resampling to improve the recall score of predictions for beers with an overall review of 3 and under.

#### Slides 
**Presentation is drafted in Google Slides**
(https://docs.google.com/presentation/d/16uvX4NDOVZA92_KLJNtno265sSpNJKDcykty3R15uHI/edit?usp=sharing)

Presentations are finalized in Google Slides.
1. Slides are primarily images or graphics (rather than primarily text) 

**2. Images are clear, in high-definition, and directly illustrative of subject matter**

#### Live Presentation 
1. All team members present in equal proportions 
2. The team demonstrates interactivity of dashboard in real time 
3. The presentation falls within any time limits provided by instructor 
4. Submission includes speaker notes, flashcards, or a video of the presentation rehearsal
 
### GitHub
#### Main Branch 
**1. All code in the main branch is production-ready.**

**2. All code necessary to perform exploratory analysis**

**3. All code necessary to complete machine learning portion of project**

**4. All code is clean, commented, easy to read, and adheres to a coding standard (e.g., PEP8)**

5. Any images that have been created (at least three) 
6. Requirements.txt file

#### README.md  

**1. Description of the communications protocols**

**2. Outline of the project (this may include images, but should be easy to follow and digest)**

**3. Cohesive, structured outline of the project (this may include images, but should be easy to follow and digest)**

4. Link to dashboard (or link to video of dashboard demo) 

**5. Link to Google Slides presentation**

https://docs.google.com/presentation/d/16uvX4NDOVZA92_KLJNtno265sSpNJKDcykty3R15uHI/edit?usp=sharing

Note: The descriptions and explanations required in all other project deliverables should also be in your README.md as part of your outline, unless otherwise noted.

#### Individual Branches 
**1. At least one branch for each team member**

**2. Each team member has at least four commits for the duration of the final segment (8 total commits per person)**

**3. Each team member has at least four commits for the duration of the final segment (16 total commits per person)**

### Machine Learning Model
Team members present a provisional machine learning model that stands in for the final machine learning model and accomplishes the following:

**1. Takes in data in from the provisional database**

      - beer_reviews.csv
      
**2. Outputs label(s) for input data**

    - review_aroma
    - review_appearance
    - review_palate
    - review_taste
    - beer_abv
    - Target variable = review_overall (3 or under, or 3.5 or higher)

**Team members submit the working code for their machine learning model, as well as the following:**

    - See attached Logistic Regression and Random Forest Jupyter Notebooks
    - See Google slide deck for the below 1-7 deliverables
1. Description of data preprocessing 
2. Description of feature engineering and the feature selection, including the team's decision-making process 
3. Description of how data was split into training and testing sets 
4. Explanation of model choice, including limitations and benefits 
5. Explanation of changes in model choice (if changes occurred between the Segment 2 and Segment 3 deliverables) 
6. Description of how model was trained (or retrained, if they are using an existing model) 
7. Description and explanation of model’s confusion matrix, including final accuracy score

**Additionally, the model obviously addresses the question or problem the team is solving.**

Note: If statistical analysis is not included as part of the current analysis, include a description of how it would be included in the next phases of the project.

 
### Database
Team members present a final project with a fully integrated database. 

**1. Database stores static data for use during the project**

      - https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate
      
**2. Database interfaces with the project in some format (e.g., scraping updates the database, or database connects to the model)**

3. Includes at least two tables (or collections, if using MongoDB) 
4. Includes at least one join using the database language (not including any joins in Pandas) 
5. Includes at least one connection string (using SQLAlchemy or PyMongo) 

Note: If you use a SQL database, you must provide your ERD with relationships.


### Dashboard
A blueprint for the dashboard is created and includes all of the following:

1. Storyboard on Google Slide(s) 

**2. Description of the tool(s) that will be used to create final dashboard**

      - Tableau Desktop
      
**3. Description of interactive element(s)**

      - Show the breweries and average overall review. Allow the user to select a set of breweries and/or an overall review range.
      - Show the average overall review by ABV. Allow the user to select an ABV range and/or beer style.


The dashboard presents a data story that is logical and easy to follow for someone unfamiliar with the topic. It includes all of the following:
1. Images from the initial analysis 
2. Data (images or report) from the machine learning task 
3. At least one interactive element

Either the dashboard is published or the submission includes a screen capture video of it in action. 

Working Notes
- Data at a glance: overview tab to give the user a good idea of how much data, what kind of data, etc they are seeing
- Brewery tab: ability to check one or multiple breweries and toggle a review slider to see  reviews by brewery, beer type and reviewer
- Beer tab: ability to check one or more beer types and toggle a review slider to see overall reviews, reviews by taste, aroma, flavor, etc.
- ABV tab: ability to check one or more ABV level and a toggle a review slider to see overall reviews, reviews by brewery and review by taste
