DATA SCIENCE CAPSTONE PROJECT
 
                Dawit Zerihun

Project Description, background, objectives, and Project Type

   Project Description:
 
   • This folder contains the results of a final capstone project submitted by the author as part of the requirement for the 
     Professional Certificate in Data Science from Coursera-IBM (Completed on April 7, 2026)

   Project Background and Context:

   • Commercial space exploration
     - The commercial space age has arrived
     - Companies are competing to make space exploration, travel, and delivery of payloads to space accessible and affordable

   • SpaceX stands out for its achievements among private space companies
     - Sending and returning space craft to the international space station
     - Launching Starlink satellite constellations
     - Conducting manned space missions

   • SpaceX innovation and efficiency
     - SpaceX pioneered a technology that enables it to reuse the first stage of its rockets
     - Resultant cost saving allowed SpaceX to advertise its service price on its Falcon 9 rocket launches for $62 million
     - Competitors’ price exceed $165 million

   Problem Description and Objectives:

   • Problem description
     - A new space exploration company plans to develop a major program that competes with SpaceX
     - As part of its efficiency drive the new company seeks to build a machine Learning (ML) model with the specifications:
        Capable of accurately predicting landing outcomes (success or failure) for the first stage of SpaceX’s Falcon 9 rocket
        Capable of evaluating the effects of prediction accuracy of the model on the new company’s pricing strategy of its rocket launch services
        Public domain data on SpaceX's Falcon 9 rocket will be used for model development
 
   • Objectives
     - Develop a machine learning model for the new company
     - Advise the new company on landing success rates of its rocket launches and implications on pricing strategy

   • The type of machine learning problem: The problem involves predicting discrete categories - specifically binary outcomes on SpaceX's
                                           Falcon 9 rocket landing success or failure, based on labeled historical data. It is a
                                           classification problem and, hence, falls under supervised machine learning category

Files and Folders

Subfolder and files:
• The data science capstone project folder contains 4 subfolders and 10 files

Types of files:
• Interactive Python Notebooks (*.ipynb) created with Jupyter notebook:  Contain Python Code, pandas dataframes, charts, comments/discussions, SQL code
• Web-based interactive dashboards with Plotly-Dash:                     Contains a zipped folder with *.png files. Each png file displays images of a dashboard setting and comments   
• Portable Document Format (PDF) files:                                  Contains a Plotly-Dash code for dashboarding
• Web-based interactive Folium maps:                                     Contains zipped folder with *.png files. Each png file displays image of georeferenced SpaceX landing data and discussion
• PDF file:                                                              Contains project report

Subfolders, files, and description:

a) Files in Subfolder "Data collection and Preprocessing" :                   A subfolder with 3 files. The files in this subfolder retrieve SpaceX data from source websites, import data into
                                                                              pandas dataframe, perform data processing, and upload data to a repository - perform ELT operation

     - Data Collection SpaceX API Falcon 9 Landing Prediction.ipynb:          An Interactive Python Notebook (ipynb) used to retrieve historical SpaceX data from the SpaceX REST API website using
                                                                              an API. Data was loaded to a dataframe, preprocessed, and was exported to repository as *.csv file

     - Web Scraping Wikipedia SpaceX Falcon 9 Landing Prediction.ipynb:       An Interactive Python Notebook (ipynb) used to retrieve historical data, on Falcon 9 and Falcon Heavy launch records of
                                                                              SpaceX, from a Wikipedia site through web scrapping. The data, which was in html format, was parsed using the BeautifulSoup
                                                                              library of Python and all occurrences of data tables in the parsed content were stored in a Python list. Contents of the
                                                                              tables were then extracted and imported into pandas dataframe. Data was preprocessed and exported to a repository as *.csv file

      - Data Wrangling SpaceX Falcon 9 Landing Prediction.ipynb:              An Interactive Python Notebook (ipynb) used Python code to import input data (specifically, data collected from SpaceX API)
                                                                              from the repository. The imported data (which is in *.csv format) was loaded into a dataframe for further processing, which
                                                                              include: 
                                                                                      Data cleaning, detection and handling null values and outliers 
                                                                                      Checking data types for possible type casting 
                                                                                      Data understanding - explore potential features and significance in terms of their effect on rocket landing outcomes, and 
                                                                                      Creating a dependent variable column, populating it with binary integer labels, and assessing the existence/absence of 
                                                                                       class imbalance

b) Files in Subfolder "Data Preparation and Feature Selection" :              A subfolder with 2 files. The files in this subfolder retrieve SpaceX data (in *.csv format) import the data into a dataframe,
                                                                              perform data analysis and feature selection, and upload data to a repository

     - Exploratory Data Analysis with SQL.ipynb:                              An Interactive Python Notebook (ipynb) used Python code to retrieve SpaceX data from a repository (as *.csv file). The data was then 
                                                                              read into a dataframe. A SQL table was created from the dataframe in IBM's DB2 database and a connection was established to the database. 
                                                                              The notebook was then used to further execute a series of SQL queries to enhance data understanding

     - Exploratory Data Analysis with Visualization.zip:                      A zipped folder with 16 image (*.png) files. Each file in this folder contains a Jupyter cell or a couple of cells with Python code,
                                                                              comments/discussion, or charts. Python code is used to retrieve preprocessed SpaceX data - specifically, data processed in the data
                                                                              Wrangling phase. The data (which is imported in a *.csv format) was then loaded into a dataframe and analyzed using visualization tools
                                                                              (matplotlib.pyplot and seaborn). Results of the data analysis coupled with considerations of hardware and related factors was used in the
                                                                              selection of predictor variable set. Based on which, a dataframe containing the feature set and the dependent variable was created.
                                                                              Categorical features were then transformed into integer labels using one-hot encoding technique. Data was checked for the presence of
                                                                              null values. The data set which is ready for predictive analysis was then uploaded to a repository in *.csv format

c) Files in Subfolder "Interactive Visual Analytics" :                        A subfolder with 3 files. The files in this subfolder use SpaceX data to create web based interactive visualization tools for displaying 
                                                                              the landing outcomes and success rates of SpaceX Falcon-9 rockets

     - Interactive Visual Analytics with Folium.zip:                          A zipped folder with 20 image (*.png) files. Each file in this folder contain Jupyter cells with Python code, comments/discussion, or maps. 
                                                                              The Python code blocks in these files were used to retrieve preprocessed SpaceX data, including coordinates of launch sites and associated 
                                                                              number of launches and landing outcomes. Launch sites were shown on a Folium (a python geospatial data visualization library) map using                                                                                       location markers. Landing outcomes in each launch site were then displayed on the map as marker clusters. Map was also used to conduct  
                                                                              proximity analysis of launch sites to infrastructure, coastline, and urban centers 
 
     - Interactive Visual Analytics with Plotly-Dash.zip:                     A zipped folder with 7 image (*.png) files. Each file in this folder represents a sample chart generated by a web-based interactive Plotly-Dash
                                                                              dashboard depicting landing success rates and counts for each launch site. The charts also display comparison of landing success rate between                                                                                 sites

     - Plotly-Dash Code for Interactive Dashboard.pdf:                        A PDF file containing the Plotly-Dash code used to create the interactive dashboard
 
 
d) Files in Subfolder "Predictive Analytics and Project Report":              A subfolder with 2 files. This subfolder contains a zipped folder with a set of files describing model development, testing, and refinement  
                                                                              process (consisting of code blocks, charts, and discussion) and a file that presents the project report

     - Predictive Analytics with Machine Learning Models:                     A zipped folder with 32 image (*.png) files. Each file in this folder contain Jupyter cells with Python code, comments/discussion, or charts.                                                                                 The .png files present the steps followed in the development, testing, and refinement of four alternative machine learning models - Logistic   
                                                                              Regression, Support Vector Machine, Decision Tree, and K-Nearest Neighbor models. Model selection among the alternatives was discussed and 
                                                                              limitations of the study along with recommendations for a follow up study were highlighted

     - ds-capstone-project-Coursera-IBM-program.pdf:                          The file presents a comprehensive project report, which was prepared as MS Power Point slides and was then uploaded to GitHub in PDF format
 

_________________

Note: Some project files were uploaded as zipped folders containing *.png files, because the author was unable to extract the corresponding *.ipynb files from the Jupyter notebooks.
      TO VIEW THESE FILES YOU MAY NEED TO DOWNLOAD THE ZIPPED FOLDER TO YOUR LOCAL DRIVE, BY CLICKING ON VIEW RAW   
 
