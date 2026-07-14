### **DATA SCIENCE CAPSTONE PROJECT**

&#x20;

&#x20;               **Dawit Zerihun**



##### **Project Description, background, objectives, and Project Type**



&#x20;  **Project Description**:

&#x20;

&#x20;  • This folder contains the results of a final capstone project submitted by the author as part of the requirement for the 

&#x20;    *Professional Certificate in Data Science from Coursera-IBM (Completed on April 7, 2026)*



&#x20;  **Project Background and Context:**



&#x20;  • Commercial space exploration

&#x20;    *- The commercial space age has arrived*

&#x20;    *- Companies are competing to make space exploration, travel, and delivery of payloads to space accessible and affordable*



&#x20;  • SpaceX stands out for its achievements among private space companies

&#x20;    - *Sending and returning space craft to the international space station*

&#x20;    *- Launching Starlink satellite constellations*

&#x20;    *- Conducting manned space missions*



&#x20;  • SpaceX innovation and efficiency

&#x20;    *- SpaceX pioneered a technology that enables it to reuse the first stage of its rockets*

&#x20;    *- Resultant cost saving allowed SpaceX to advertise its service price on its Falcon 9 rocket launches for $62 million*

&#x20;    *- Competitors’ price exceed $165 million*



&#x20;  **Problem Description and Objectives:**



&#x20;  • Problem description

&#x20;    - *A new space exploration company plans to develop a major program that competes with SpaceX*

&#x20;    *- As part of its efficiency drive the new company seeks to build a machine Learning (ML) model with the specifications:*

&#x20;       *Capable of accurately predicting landing outcomes (success or failure) for the first stage of SpaceX’s Falcon 9 rocket*

&#x20;       *Capable of evaluating the effects of prediction accuracy of the model on the new company’s pricing strategy of its rocket launch services*

&#x20;       *Public domain data on SpaceX's Falcon 9 rocket will be used for model development*

&#x20;

&#x20;  • Objectives

&#x20;    - *Develop a machine learning model for the new company*

&#x20;    *- Advise the new company on landing success rates of its rocket launches and implications on pricing strategy*



&#x20;  • The type of machine learning problem: *The problem involves predicting discrete categories - specifically binary outcomes on SpaceX's*

&#x20;                                          *Falcon 9 rocket landing success or failure, based on labeled historical data. It is a*

&#x20;                                          *classification problem and, hence, falls under supervised machine learning category*



#### **Files and Folders**

#### 

**Subfolder and files**:

• The data science capstone project folder contains 4 subfolders and 10 files



**Types of files:**

• Interactive Python Notebooks (\*.*ipynb*) created with Jupyter notebook:  Contain *Python Code, pandas dataframes, charts, comments/discussions, SQL code*

• Web-based interactive dashboards with Plotly-Dash:                     Contains a zipped folder with *\*.png* files. Each *png* file displays images of a dashboard setting and comments   

• Portable Document Format (PDF) files:                                  Contains a *Plotly-Dash code for dashboarding*

• Web-based interactive Folium maps:                                     Contains zipped folder with *\*.png* files. Each *png* file displays image of georeferenced SpaceX landing data and discussion

• PDF file:                                                              Contains *project report*



**Subfolders, files, and description:**



*a) Files in Subfolder* "Data collection and Preprocessing" :                   *A subfolder with 3 files*. The files in this subfolder retrieve SpaceX data from source websites, import data into

&#x20;                                                                             pandas dataframe, perform data processing, and upload data to a repository - perform ELT operation



&#x20;    - *Data Collection SpaceX API Falcon 9 Landing Prediction.ipynb:*          *An Interactive Python Notebook (ipynb)* used to retrieve historical SpaceX data from the SpaceX REST API website using

&#x20;                                                                             an API. Data was loaded to a dataframe, preprocessed, and was exported to repository as *\*.csv* file



&#x20;    - *Web Scraping Wikipedia SpaceX Falcon 9 Landing Prediction.ipynb:*       *An Interactive Python Notebook (ipynb)* used to retrieve historical data, on Falcon 9 and Falcon Heavy launch records of

&#x20;                                                                             SpaceX, from a Wikipedia site through web scrapping. The data, which was in *html* format, was parsed using the BeautifulSoup

&#x20;                                                                             library of Python and all occurrences of data tables in the parsed content were stored in a Python list. Contents of the

&#x20;                                                                             tables were then extracted and imported into pandas dataframe. Data was preprocessed and exported to a repository as *\*.csv* file



&#x20;     - *Data Wrangling SpaceX Falcon 9 Landing Prediction.ipynb:*              *An Interactive Python Notebook (ipynb)* used Python code to import input data (specifically, data collected from SpaceX API)

&#x20;                                                                             from the repository. The imported data (which is in \*.csv format) was loaded into a dataframe for further processing, which

&#x20;                                                                             include: 

&#x20;                                                                                     Data cleaning, detection and handling null values and outliers 

&#x20;                                                                                     Checking data types for possible type casting 

&#x20;                                                                                     Data understanding - explore potential features and significance in terms of their effect on rocket landing outcomes, and 

&#x20;                                                                                     Creating a dependent variable column, populating it with binary integer labels, and assessing the existence/absence of 

&#x20;                                                                                      class imbalance



*b) Files in Subfolder* "Data Preparation and Feature Selection" :              *A subfolder with 2 files*. The files in this subfolder retrieve SpaceX data (in \*.csv format) import the data into a dataframe,

&#x20;                                                                             perform data analysis and feature selection, and upload data to a repository



&#x20;    - *Exploratory Data Analysis with SQL.ipynb:*                              *An Interactive Python Notebook (ipynb)* used Python code to retrieve SpaceX data from a repository (as *\*.csv* file). The data was then 

&#x20;                                                                             read into a dataframe. A SQL table was created from the dataframe in IBM's DB2 database and a connection was established to the database. 

&#x20;                                                                             The notebook was then used to further execute a series of SQL queries to enhance data understanding



&#x20;    - *Exploratory Data Analysis with Visualization.zip:*                      *A zipped folder with 16 image (\*.png) files.* Each file in this folder contains a Jupyter cell or a couple of cells with Python code,

&#x20;                                                                             comments/discussion, or charts. Python code is used to retrieve preprocessed SpaceX data - specifically, data processed in the data

&#x20;                                                                             Wrangling phase. The data (which is imported in a \*.csv format) was then loaded into a dataframe and analyzed using visualization tools

&#x20;                                                                             (matplotlib.pyplot and seaborn). Results of the data analysis coupled with considerations of hardware and related factors was used in the

&#x20;                                                                             selection of predictor variable set. Based on which, a dataframe containing the feature set and the dependent variable was created.

&#x20;                                                                             Categorical features were then transformed into integer labels using one-hot encoding technique. Data was checked for the presence of

&#x20;                                                                             null values. The data set which is ready for predictive analysis was then uploaded to a repository in \*.csv format



c) *Files in Subfolder* "Interactive Visual Analytics" :                        *A subfolder with 3 files*. The files in this subfolder use SpaceX data to create web based interactive visualization tools for displaying 

&#x20;                                                                             the landing outcomes and success rates of SpaceX Falcon-9 rockets



&#x20;    - *Interactive Visual Analytics with Folium.zip:                          A zipped folder with 20 image (\*.png) files.* Each file in this folder contain Jupyter cells with Python code, comments/discussion, or maps. 

&#x20;                                                                             The Python code blocks in these files were used to retrieve preprocessed SpaceX data, including coordinates of launch sites and associated 

&#x20;                                                                             number of launches and landing outcomes. Launch sites were shown on a Folium (a python geospatial data visualization library) map using location 

&#x20;                                                                             markers. Landing outcomes in each launch site were then displayed on the map as marker clusters. Map was also used to conduct proximity analysis 

&#x20;                                                                             of launch sites to infrastructure, coastline, and urban centers 

&#x20;

&#x20;    - *Interactive Visual Analytics with Plotly-Dash.zip:                     A zipped folder with 7 image (\*.png) files.* Each file in this folder represents a sample chart generated by a web-based interactive Plotly-Dash

&#x20;                                                                             dashboard depicting landing success rates and counts for each launch site. The charts also display comparison of landing success rate between sites



&#x20;    - Plotly-Dash Code for Interactive Dashboard.pdf:                        A PDF file containing the Plotly-Dash code used to create the interactive dashboard

&#x20;

&#x20;

d) *Files in Subfolder* "Predictive Analytics and Project Report":              *A subfolder with 2 files*. This subfolder contains a zipped folder with a set of files describing model development, testing, and refinement process 

&#x20;                                                                             (consisting of code blocks, charts, and discussion) and a file that presents the project report



&#x20;    - Predictive Analytics with Machine Learning Models:                     A *zipped folder with 32 image (\*.png) files.* Each file in this folder contain Jupyter cells with Python code, comments/discussion, or charts. The 

&#x20;                                                                             *.png* files present the steps followed in the development, testing, and refinement of four alternative machine learning models - Logistics Regression, 

&#x20;                                                                             Support Vector Machine, Decision Tree, and K-Nearest Neighbor models. Model selection among the alternatives was discussed and limitations of the study 

&#x20;                                                                             along with recommendations for a follow up study were highlighted



&#x20;    - ds-capstone-project-Coursera-IBM-program.pdf:                          The file presents a comprehensive project report, which was prepared as MS Power Point slides and was then uploaded to GitHub in PDF format

&#x20;



\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_



Note: Some project files were uploaded as *zipped folders containing \*.png files*, because the author was unable to extract the corresponding *\*.ipynb file*s from the Jupyter notebooks

&#x20;

