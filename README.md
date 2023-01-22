# prison_mike_analysis AKA BEER REVIEWS

## Notes
- Data cleaning & parsing
  - ETL (could be multiple tables)
  - postgres/SQL
- Visualization - Tableau
- Machine learning
- Presentation

## Things mentioned in class
- A database can be any place you save and store your data - local machine or in something like PostGres
- For each team member to get in a specific amount of commits, whatever section they are responsible for can be broken into small tasks that are then pushed as new commits
- Each section of the project does not need to be completed or brainstormed linearly
  - for example: ML model can be brainstormed and mocked up at the same time the database is created
    
  ## Group Assignments
  Brad
  - clean, data insights, python etc
  
  Noa
  - tableau, visualizations

  Sanjay
  - machine learning, database erd

Emily
  - Machine learning, a little data cleanng, project manager

## Week 1 Deliverables
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
 - Sample data that mimics the expected final database structure or schema 
 - Draft machine learning module is connected to the provisional database
