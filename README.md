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
 - integrated database
 - at least 2 tables, 1 join, 1 connection string
- Dashboard
  - Data story that is logical and easy to follow
  - Images from the initial analysis
  - Data from the machine learning task
  - At least one interactive element

## Project Notes
- Our data source file is over 200MB. Over 30MB when zipped. We attempted lfs and were not successful. Please see this link for our data.
https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate
- We chose to use the initial csv (after cleaning) as our database. We created a mockup ERD only.

## Group Assignments & Communication Protocols
### Assignments
 - Brad: clean, data insights, python, google slides collaboration
 - Noa: tableau visualizations, data insights, google slides collaboration
 - Sanjay: data cleaning, machine learning model and reasoning, database erd, google slides collaboraton
 - Emily: data cleaning, machine learning model and reasoning, data cleanng, project manager, google slides collaboration
 
 ### Communication Protocols
  - Established a slack channel for communication
  - Met during class time and Sundays. Worked individually inbetween group meetings.

## Overall Rubric deliverables (bolded as completed)
### Content
Team members have drafted their project, including the following:
 - Selected topic:  
   - Beer Advocate Beer Reviews
 - Reason why they selected their topic:
   - Beer
   - Applicable to demographic
 - Description of their source of data
   - https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate
   - Beer Reviews from Beer Advocate (1.5 Million reviews)
   - Large data set
   
![image](https://user-images.githubusercontent.com/109913335/213871425-761738a5-4856-4646-a973-d43a5807efc1.png)

 - Questions we hope to answer with the data
   - What attributes contribute to a review over 3?
   - What breweries have the best ratings?
   - Which attribute of the review contributes the most to the overall review score?
   - Which beer style gets the best overall review?
   - Which beer style has the best aroma review scores?
   - Once a person selects a brewery, show the beers and breweries with the highest overall reviews.
   - Once a person selects an ABV bucket, show beers and breweries with the highest overall reviews.
 
### GitHub
Main Branch 
 - Includes a README.md
 - README.md README.md must include: 
   - Description of the communication protocols: 
     - Meeting on class days and Sundays.
     - Created a slack channel for group to communicate updates and questions

Individual Branches 
 - At least one branch for each team member
 - Each team member has at least four commits from the duration of the first segment

### Machine Learning Model
Team members present a provisional machine learning model that stands in for the final machine learning model and accomplishes the following:
 - Takes in data in from the provisional database
   - beer_reviews.csv
 - Outputs label(s) for input data
   - review_aroma
   - review_appearance
   - review_palate
   - review_taste
   - beer_abv
   - Target = review_overall (3 or under, or 3.5 or higher)
 
### Database
Team members present a provisional database that stands in for the final database and accomplishes the following:
 - Sample data that mimics the expected final database structure or schema:
   - https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate
 - Draft machine learning module is connected to the provisional database: See Model notebook

### Visualization - Tableau

- Data at a glance: overview tab to give the user a good idea of how much data, what kind of data, etc they are seeing
- Brewery tab: ability to check one or multiple breweries and toggle a review slider to see  reviews by brewery, beer type and reviewer
- Beer tab: ability to check one or more beer types and toggle a review slider to see overall reviews, reviews by taste, aroma, flavor, etc.
- ABV tab: ability to check one or more ABV level and a toggle a review slider to see overall reviews, reviews by brewery and review by taste
