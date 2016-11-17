## Introduction to Data Science for Public Policy 

The Introduction to Data Science for Public Policy (**PPOL 670-01**) is a survey course of the fundamentals of data science.  The course is focused on evaluating and analyzing public policy, telling stories with data to make compelling and fact-based arguments.  


The objective of the course to equip students with the skills to tell stories with data and drive action.  Public policy is part of a large and sprawling social system.  Parsing causality from a system of variables where everything is related requires a scalpel.  This refined approach can be assembled from pre-written code and routines; but it still requires skilled assembly.  We will teach an approach that leverages analytical routines that have already been written.  The value of this course is in the mortar, not the bricks.  


#### Instructors

**Jeff Chen** is the Deputy Chief Data Officer and was the first Chief Data Scientist of the U.S. Department of Commerce. He has led wide ranging initiatives across 30+ fields, ranging from emergency services to international public health to legal affairs to trade economy. Jeff has previously served as the Director of Analytics at the NYC Fire Department leading development of fire prediction algorithms, senior data roles in the NYC Mayor’s Office during the Bloomberg Administration focusing on city operations and health + human services, and an advisor to governments, corporations, and non-profits on applied data for strategy and operations.


Jeff and Dan worked together as White House Presidential Innovation Fellows at NASA.  


**Dan Hammer** is now a Senior Policy Advisor at the White House, where he works with the U.S. Chief Technology Officer and U.S. Chief Data Scientist on the public finance of data infrastructure.  He was previously the Chief Data Scientists at two environmental non-profits.  He cofounded Global Forest Watch, a web application to monitor forests from satellite imagery.  He is a Fellow at the Berkeley Institute for Data Science and a PhD candidate in environmental economics at UC Berkeley.  


#### Time and location

Mondays, 6:30pm to 9:00pm

1. January 11 (Wednesday)
2. January 23
3. January 30
4. February 6
5. February 13
6. February 27 
7. March 13
8. March 20
9. March 27
10. April 3
11. April 10
12. April 24 
13. May 1

### Course outline

#### Section 1: Fundamentals

Data science is about designing and building data products that derive insight. This first section will focus on developing fundamental skills required to build effective products.

##### Lecture 1: Preliminaries

The objective of the first lecture is to overcome the coefficient of static friction in using R for data science.  Students will learn to execute simple R scripts to read, write, and extract data elements.


###### Lecture objectives

1. Why code matters
2. Set up, edit, and save RMarkdown 
3. Getting started with Github
4. Read data from CSV and JSON
5. Data types and classes, including matrix, data.frame, list, and vectors
6. Extracting rows, columns, and specific elements from a data frame
7. Basic operations (e.g., sum, mean) on rows; useful as consistency checks.
8. Write data to CSV and JSON


###### Example application

- Health from the Demographic and Health Surveys or Census data.


##### Lecture 2: Data manipulation

The objective of this lecture is to present the most important and fundamental elements of data manipulation.  These core operations include sort, merge, reshape, and collapse.  We will also present loops through multiple rows or columns, and other alternatives to operate on partitions of data frames.

###### Lecture objectives

1. Mastery of data manipulation makes for good data scientists
2. Sort data based on column values
3. Subset data frames
4. Reshape data table, wide ⇔ long
5. Merge data frames
6. Collapse data frames
7. Text processing: capitalization, substring, regex
8. Looping through basic operations (bonus: same idea without loops)


###### Example application

- Collapse data at the county level to state level
- Process NYC 311 data from point level to Census tract level


##### Lecture 3: Data quality and re-usable code

The objective of this lecture is to handle missing values appropriately and script visual checks to find errors introduced in data input/output.  We will also start to view computational optimization techniques, like taking advantage of multiple cores for heavy duty operations (parallel processing).


###### Lecture objectives

1. A data scientist’s work is only as good as data quality
2. Handling missing values and their properties
3. Replacing values by condition
4. Visual checks: hist(), plot(), ggplot2
5. Writing functions

###### Example applications	

- GHCN-M: Missing values analysis in matrix of weather anomalies from 1880 to Present
- Weather: Matching human-reported weather events to radar events over time and space


##### Lecture 4: Exploratory Data Analysis
[ ]


###### Lecture objectives

1. 

###### Example applications	

-


##### Section 2: Data Analysis + Modeling

The use case drives the technique. In public policy, data can be used to support evaluation of programs to understand causal mechanisms (e.g. retrospective focus) or enable the creation of data-rooted products that drive action (e.g. deployed applications). Machine learning and data analysis enables both uses of data and will be the focus of the next five courses

###### Lecture 5: Introduction to Supervised Learning 

Supervised learning is the most relied upon class of techniques that enable causal inference but also deployed precision policy. How does changing one variable independently impact another variable?  We begin to introduce basic regression analysis, correlation coefficients, ordinary least squares, and the relationship between the concepts.  Note that this is a very cursory review, and the deep assumptions are not tested or expounded upon.

###### Lecture objectives

1. Three common data science problems in public policy: 
2. Supervised: Scoring or prediction for application
3. Supervised: Causal inference and evaluation for understanding
4. Unsupervised: Clustering for structure
5. What is supervised learning?
6. Structure of a supervised learning project
7. Target variables, Input variables, Objective function and evaluation measures, model experiment design, Cross validation versus train/validate/test,  Regression versus classifiers
8. Ordinary Least Squares (OLS): Graphical illustration 
9. Linear models in `R`
10. Exporting results tables
11. The limits of correlation coefficients and R-squared statistics
12. Introduction to scoring and prediction: train/validate/test

###### Example application	

- Labor and wage analysis, innate ability. (David Card data set.)
- Economic data from BEA

##### Lecture 6: Simulations, selection bias 

Formal statistics offers methods to calculate closed-form, analytical answers to the limits of OLS regression.  Data science offers a more immediate and arguably a more accessible solution: simulate conditions and examine the outcomes.  We begin to use the early visualizations techniques taught in a previous lecture for analysis.

###### Lecture objectives
1. Simulating OLS and identifying p-values
2. For-loops versus `apply` for simulations
3. Visualizing distributions with ggplot

###### Example application	

- TBD

##### Lecture 7: Regression discontinuity and difference-in-difference estimation

An introduction to assessing the causal impact of public policy.

###### Lecture objectives

1. Interpretation of dummy variables
2. Difference-in-differences (DiD) as a causal estimator
3. Assumptions and potential issues with DiD
4. Regression discontinuity (RD) analysis
5. Visualizing RD analysis

###### Example application	

- TBD

##### Lecture 8: Classification techniques 

Classification models are one of the workhorses of data science. Classifiers enables data-driven applications such as risk scoring, lawsuit outcome prediction, marketing lead generation, facial detection and computer vision, spam filtering, among other use cases.  This session will focus on the fundamentals of classification models, types of models, and daily applications.

###### Lecture objectives
1.	Three common problems using classifiers
2.	Structure of a classification project
Target variables, Input variables, Objective function and evaluation measures, model experiment design, Cross validation versus train/validate/test
Confusion matrix, TPR, TNR, AUC
3.	Framing dataset
4.	Models: statistical assumptions and mechanics, risks/strengths, implementation, non-technical explanation, Decision trees, Logistic Regression, K-Nearest Neighbors
5.	Appropriate uses of classification techniques, Scoring, prediction and prioritization, Propensity score matching


###### Example application	

- Credit Card Default Dataset (UCI/Kaggle)

##### Lecture 9: Unsupervised learning 

No, this is not an independent study session. Unsupervised learning techniques such as clustering and principal components analysis helps to identify recognizable patterns when no labels are provided. In sales and recruitment offices, customer segmentation may use current customer data, then use clustering techniques to identify k-number of distinct customer profiles. In resourceful law firms, data scientists may develop topic modeling algorithms to automatically tag and cluster hundreds of thousands of documents for improved search. This session will focus on clustering methodologies that are commonly employed in applied research.

###### Lecture objectives

1.	Three common problems using unsupervised learning 
2.	Structure of unsupervised learning project, Input variables, optimization methods
3.	Framing dataset
4.	Models: statistical assumptions and mechanics, risks/strengths, implementation, sanity checks, non-technical explanation, K-means clustering (K-means), Principal Components Analysis (PCA)/Dimensionality Reduction, Hierarchical clustering (if time permits)
5.	Appropriate uses of k-means and PCA

###### Example application(s)

- Univariate clustering application: k-means
- Multivariate clustering application: Customer segmentation using Census American Community Survey


#### Section 3: Data enhancement and visualization

Beyond the data preparation and modeling, the ‘presentation layer’ is the glue that will allow a data science project stick with target audiences. Often times, presentation is graphical and relies upon a rich ecosystem of visualization, web services, and interactive applications to communicate pertinent issues.

##### Lecture 10: Data storytelling through graphical representation

Often times, the model is not enough to communicate the value of the data analysis. A well-designed visualization can illustrate patterns and allow target audiences to establish a connection with the analytical effort at hand. 

###### Lecture objectives

1. Three examples of the presentation layer
2. Static visualizations: ggplot2
3. Interactive visualizations: dygraphs, plotly, networkd3, threejs

###### Example application	

- Phone gyroscopic data: time series
- Global trade flows: network map


##### Lecture 11: Web service APIs and spatial data

There are many cases where you will rely on data or services that aren’t stored or build on your local machine, but rather are exposed as web service application programming interfaces (APIs).  These are the components of modern software development, and we will teach how to find and utilize these services from within the R programming environment.  We use this lecture as an opportunity to introduce spatial data within R by interacting with an API for geographic data.

###### Lecture objectives

1. 	Three examples of APIs and why they matter
2.	Interacting with web service APIs from R
3.	Writing a client-side function to simplify the remote interaction
4.	Batch request for elevation data from the Google Elevation API
5.	Viewing the spatial data in R


###### Example application	

- Extracting elevation data from the Google Elevation API
- Identifying the characteristics of farmers’ markets in the Southwest United States.


##### Lecture 12:  Spatial Data and Maps

The state of data is rapidly expanding in two principal directions: transactional-level and spatially. Maps are the principal mode of representing spatial data, which relies upon different types of GIS formats (e.g. shapefiles, raster, GeoJSON) and presentation medium. This lecture dives into spatial considerations in data science.

###### Lecture objectives

1. 	Three examples of spatial data
2.	A framework for approaching GIS
3. 	Preliminaries of GIS data, File types (shp, .nc, .tif, .json), Projections, Feature type (point, line, polygons, grids), Visualizations (choropleth, dot density, proportional)
4.	Mapping choropleth maps using polygon shapefiles
5.	Geoprocessing of points to polygon
6.	Displaying multiple layers

###### Example application	

- Chicago crime data


##### Lecture 13:  Export results and interactivity

Often times, users like to interact with a product as opposed to reading curated results. Enter interactivity -- a well-proven mode of displaying results.

###### Lecture objectives

1. 	Three examples of interactive data science
2.	An Intro to R Shiny 
3. 	Building a simple interactive tool

###### Example application	

- TBD
					
#### Required Text

#### Disability				

If you believe you have a disability, then you should contact the Academic Resource Center (arc@georgetown.edu) for further information. The Center is located in the Leavey Center, Suite 335 (202-687-8354). The Academic Resource Center is the campus office responsible for reviewing documentation provided by students with disabilities and for determining reasonable accommodations in accordance with the Americans with Disabilities Act (ASA) and University policies. For more information, go to http://academicsupport.georgetown.edu/disability/.
					
#### Important Academic Policies and Academic Integrity				

McCourt School students are expected to uphold the academic policies set forth by Georgetown University and the Graduate School of Arts and Sciences. Students should therefore familiarize themselves with all the rules, regulations, and procedures relevant to their pursuit of a Graduate School degree. The policies are located at: http://grad.georgetown.edu/academics/policies/
					
#### Provosts Policy Accommodating Students Religious Observances			

Georgetown University promotes respect for all religions. Any student who is unable to attend classes or to participate in any examination, presentation, or assignment on a given day because of the observance of a major religious holiday (see below) or related travel shall be excused and provided with the opportunity to make up, without unreasonable burden, any work that has been missed for this reason and shall not in any other way be penalized for the absence or rescheduled work. Students will remain responsible for all assigned work. Students should notify professors in writing at the beginning of the semester of religious observances that conflict with their classes. The Office of the Provost, in consultation with Campus Ministry and the Registrar, will publish, before classes begin for a given term, a list of major religious holidays likely to affect Georgetown students. The Provost and the Main Campus Executive Faculty encourage faculty to accommodate students whose bona fide religious observances in other ways impede normal participation in a course. Students who cannot be accommodated should discuss the matter with an advising dean.
					
#### Statement on Sexual Misconduct

Please know that as a faculty member I am committed to supporting survivors of sexual misconduct, including relationship violence, sexual harassment and sexual assault. However, university policy also requires me to report any disclosures about sexual misconduct to the Title IX Coordinator, whose role is to coordinate the University’s response to sexual misconduct.
					
Georgetown has a number of fully confidential professional resources who can provide support and assistance to survivors of sexual assault and other forms of sexual misconduct. These resources include:

```					
Jen Schweer, MA, LPC
Associate Director
Health Education Services for Sexual Assault Response and Prevention 
(202) 687-0323
jls242@georgetown.edu
```
```					
Erica Shirley
Trauma Specialist
Counseling and Psychiatric Services (CAPS) 
(202) 687-6985
els54@georgetown.edu
```

More information about campus resources and reporting sexual misconduct can be found at http://sexualassault.georgetown.edu. 


