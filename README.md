# Data-Analytics
# Module Focus
  - role and scope of Data Analytics
  - compare and contrast different data types, common data structures and file formats
<details>
<summary> Week 1 </summary>
<br>
  
# The basic of Data
  ## What is Data Analytics
  - is to examine and transform raw data into actionable insights that guide inforemed decision-making processess within an orgarnisation.
  - key responsibilities and skills
    - Data Collection and Preparation - sourcing data, cleaning and organizing data
    - Data aanlysis - employing statistical methods, ML techniques to interpret data, Identify trends and patterns not obvious.
    - Data visualization - creating visual presentations of data eg. charts and dashboards to make complex information easily understandable.
    - Decision Support - make recommendations based on data-driven insights guiding besiness decisions
    - Collaboration and Communication - collaborate with other ddepartements to understand their data needs and effectively communicate complex data findings to non-technical stakeholders.
    - Continuous Learning and Adaptation - keeping up-to=date with latest trends and adapt to new analytiacl model and methods.

  TASK 
  - Data Analyst 
    - Maths and Stats
    - python and sql
    - data collection , data analysis, data visualisation
    - collaboration and communication, continuous learning and adaptation
         
  3 major piilars that allow analytics programs to thrive : Data, Storage and Computing power.

  ## The Analytics Process
  - The process is iterative rather than sequantial as you can return/revisit to any stage if theres a error in your data.
  - AI :
  - ML :
  - Deep Learning :
     
  ## Data Governance
  - is the slab of stone that supports the 3 pillars.
  - ensure that the organization has high-quality data and is able to effectively control that data.

    ### Analytics tools
    - automate data analysis, improving ability to acquire, clean, manipulate, visualize and analyze data.

# Understand Data
  ## Data Types
  - a data element is an attribute about a person, place. they describe characteristics of activities.
  - data type limits the values a data element can have.

  ## Structures data types
  - is tabular data like a spreadsheet.
  - character data types limits data entry to only valid characters.
  
  ## Unstructured
  - is any type of data that does not fit neatly into the tabular model.
  - eg. digital images, audio and video recordings
  - storing unstructured data
    - binary

  ## Categories of data
  - Quantitative (How much/many?) vs Qualitative Data (What/why?)
  - Discrete vs Countinuous Data
    - discreete represent measurements that cant be subdivided. eg. whole number
    - Countinuous can represent measure of average and have decimal 
    - Quantitative (can be both), but Qualitative is discrete
  - Categorical Data
    - Text data with known, finite number of categories
  - Dimensional Data
    - is an approach to arranging data to facilitate analysis.
   
  ## Common Structures
  ### Structured data
  - Tabular data is structured data with values stored in consistent manner and organized into rows and columns. facilitates aggregation
  - specify a unique key to identify values in a row

  ### Unstructured
  - is qualitative, describing the characteristics of an event or object.
  - eg. images, audio , video and descriptive text
  - machine data is common source of unstructured data as machines operates they create a digital footprint that data is unstructured
  - storage - key is a unique identifier and value is the data itself.

  ### Semi-Structured
  - is data that has structure and that is not tabular. eg Email
  - Every Email has structural components eg. recipient, sender, subject, date and time
  - body of email is unstructured text, while attachments can be anything type of file.

  ## Common File formats
  - facilitate data exchange and tool interoperability.
  - Text Files
  - Fixed-Width Files
  - JavaScript Object Notation
  - Extensible Markup Language (XML)
  - HyperText Markup Language (HTML)

# Data Preparation and Exploration
- Module focus
  - understand how to explore and acquire data
  - learn databases and need to classify and store or structure data
  - data manipulation techniques and how to manage data quality
  - fundamentals of stats and analysis techniques
 
  ## Databases and Data Acquisition
  - Two categories of databases
    - Relational - for storing and processing structured data
    - Nonrelational - 

  ### The Relational Model
  - The entity relationship diagram (ERD) is a visual of data modelling process, it shows the connection between related entities.
  - cardinality refers to the relationship between two entities.
  - unary relationship is when an entity has a connection with itself.
  - A binary relationship connects two entities
   
  ### Relational Databases
  - Relational databasess let you make operational system out of an ERD, Relational entities correspond to databases tables, and entity attributes correspond to table columns.
  - An associative table is both a table and a relationship
  - every row in a relational database must be unique
  - a prinmary key is one or more attributes that uniquely identify a specific row
  - a foreign key is or more columns in one table that points to corresponding columns in a related table, FK enforces referential integrity.
   
  RELATIONAL VS NON-RELATION
  - Relational - data consistency, security, ease of back up
  - Non-Relational - flexibility, high scalability, cost effective
   
  ### Non-Relational Databases
  - does not have a predefined strucure based or tabular data
  - examples
    - key-value database
      - key is globally unique across entire database
      - the data corresponding eith key can structured or ustructured
      - can scale to accomododate many simultaneous request without impacting perfomance.
    - Document
      - is similar to key-value database bbut the value is restricted to a specific structured format eg JSON
    - Column-Family
      - use an index to identify data in groups of related columns.
      - good ability to scale
    - Graph
      - specialize in exploring relationship between pieces of data.
      - each animal and person represent a node in the graph.

  ## Database Use cases
  ### Online Transactional Processing (OLTP)
  - handles daily transactions eg booking flight, or ordering online
  - balance the ability to write and read data efficiently

  ### Normalisation
  - is a process for structuring a database in a way that minimizes duplication of data.
  - First nomrmal form(!NF) is when every row in a table and every column contains a unique value
  - Second Normal Form(2NF) starts where 1NF leaves off, all nonprimary key values must depend on the entire primary key.
  - Third Normal Form(3NF) all columns must depend on only the primary key (highly normalized)

  ### Online Analytical Processing (OLAP)
  - focus on ability of organizations to analyze data.
  - OLAP and OLTP databases can use relational database but their structures are different.
  - OLTP balance transactional read and write perfomance, resulting in highly normalised design (3NF)
  - OLAP have denormalized design, this is wider tables distribution of data instead of multiple tables. more efficient for analytical queries to read large amount of data for single table.

   ### Schema Concepts
   - Tradictional systems require highly normalised databases, denormalized is for analytical systems.
   - A *Data warehouse* - is database thats aggregates data from many transactional systems for analytical purposes. (Facilitates analytics)
   - A *Data mart* is a subset of a data warehouse. DW server entire organization whereas DM focus on particular department within organization.
   - A *Data Lake* - stores raw data in its native format instead of conforming to a relational database structure.

  VIDEO
  - Database - relational database - record data (OLTP) - stored in tables , data is highly detailed, flexible
  - DW - used for analytical processing(OLAP) - databases send data to data warehouse via ETL process - data is summarized


|   DATABASE           |  DATA WAREHOUSE            |
| ------------ | ------------ |
| Transactions             | Analytics and reporting             |
| fresh and detailed data             | refreshed periodically and summarized             |
| slow when querying large amounts of data and slow down transactional processes   |  faster and dont interfere with any processes            |

  - Data lake - designed to capture raw data - made for large amounts of data
  - Star schema facilitate analytical processing, denormalized to improve read perfomance over large data,simple queries, data from OLTP into star create large data duplication so consume more space, DM use star 
  - snownflake - less denormalized,  complex query as tables grows, more complex, less storage, DW use snowflake

  ### Dimensionality
  - refers to the number of attributes a table has.
  - greater the attributes the greater higher the dimensionality.


  ## Data acquisition COncepts
  ### Integration
  - Data from transactional systems flow into data warehouses and data marts for analysis.
  - you retrieve, reshape, insert data to move data between operational and analytical environments. you can use variety of methods to transfer data efficiently and effectively.
  - one approach is Extract, Transform, and Load (ETL0
    1. Extract - extract data from source to staging area. goal is move data from relational database into a flat file
    2. Transform - goal reformat data from its transactional to data warehouse's analytical design
    3. Load - ensure data gets into the analytical system
   
  - ELT has speed advantages


  ### Data collection methods
  - Application Programming Interfaces(APIs)
  - Web services
  - Web Scrabing
  - Human in the loop
  - Surveys
  - Survey tools
  - Observation
  - Sampling

  ## Working with Data
  - to turn a database design into an operation database ready to accept data, you use Data Definition Language(DDL) components of SQL.
  - DDL lets you create, modify and delete tables
  - to generate insights, use Data Manipulation Language(DML) capabilities of SQL to insert, modify and retrieve information from databases.
  - DDL manage structure while DML manage data in the database

  ### Data Manipulation
  - 4 possible actions
    - Create new data
    - Read existing data
    - Update existing data
    - Delete existing data
  - CRUD operations

    Data Manipulation in SQL

    |  Operation     |  SQL Keyword     |  Description  |
    | -------------- |  --------------  |  --------------  |
    |  Create        |  INSERT          |  Creates new data in an existing table  |
    |  Read          |  SELECT          |  Retrieves data from an existing table  |
    |  Update        |  UPDATE          |  Changes existing data in an existing table  |
    |  Delete        |  DELETE          |  Removes existing data from an existing table  |



# Data Quality
- challenges of data quality
- data manipulation techniques
- applying data quality control

## Data Quality Challenges
- examining each data source and its own unique quality issues.

  ### Duplicate Data
  - occurs when data representing the same transaction is accidentally duplicated within a system.
  - resolve by prevent its creation and duplicate resolution process
  - source is having multiple data sources
 
  ### Redundant Data
  - is a function of intergrating multiple systems.
  - happens when same data exist in multiple places, also inaapropriate database design.
  - shared data elements
  - resolving redundant data
    - synchronization to shared data elements
    - resturcture tables
   
  ### Missing Values (Null Values)
  - impacts data quality
  - occur when you expect an attribute to contain data but nothing is there.
  - A null value is an absent of a value
  - to handle missing values, first check their existence.
 
  ### Invalid Data
  - are values outside the valid range for a given attribute.
  - violates a business rule instead of having a incorrect data type e.g for temperature -99 999 is a valid number but not a valid temperature in Earth.
 
  ### Nonparametric Data
  - is data collected from cater=gorical variables.
  - categories differ it can indicate differentiation or rank order associated eg. rank pain in a scale of 0 to 10.
 
  ### Data Outliers
  - is a value that differs significantly from other observations in a dataset.
 
  ### Specicification mismatch
  - describes the target value for a component
  - occurs when an individual components characteristics are beyond the range of acceptable values.
 
  ### Data type Validation
  - ensures that values in a dataset have a consistent data type.

  ## Data Manipulation Techbiques
  ### Recoding Data
  - is a technique to map original values for a variable into new values to facilitate analysis.
  - recoding group data into multiple categories, creating categorical variable
    - Nominal - variable with 2 or more categories with no natural order of categories eg hair color
    - Ordinal - category with an inherent rank eg T-shirt size
    - variable values fit into fixed numner of categories

  ### Derived variables
  - is a new varible resulting from a calculation on an existing variable.
  - dont have to be categorical
 
  ### Data Merge
  - uses a common variable combine multiple datasets with different structures into a single dataset.
  - improve data quality
 
  ### Data Blending
  - combines multiple sources of data into a single dataset at the reporting layer.
  - allows analyst to combine datasets in ad hoc manner without saving blended sataset in a relational database.
  - blended satasset exist only at the reporting layer
 
  ### Concatenation
  - merging of separe variables into a single variable.
 
  ### Data append
  - combines multiple data sources with the same structure, resulting in a new dataset containing all rows from the original datasets.
  - f
 
  ### Imputation
  - is a technique for dealing with missing values by replacing them with substitutes.
  - approaches to handle missing data
    - Remove missing data (Rows)
    - Replace with Zero
    - Replace with Overall average
    - Replace with Most Frequent(MODE)
    - Closest value average
   
  ### Reduction
  - is the process of shrinking an extensive dataset without begatively impacting its analytical value.
  - types
    - dimensionality reduction
      - reduction technique is dimensionality reduction which removes attributes from a dataset.
        - removing attributes reduces dataset overall size.
    - numerosity reduction
      - reduces overall volume of data. eg. using histogram
      - improve efficiency of analysis.
    - sampling
      - is a technique that selects a subset of individual records from their initial dataset.

  - Aggregation - is the summarization of raw data for analysis and control of privacy. eg finding max or min of data
  - Transposing data - is swaping rows and columns to facilitate analysis.
  - Normalization - converts data from different scales to same scale.
  - Min-Max Normalization -
  - Parsing/String Manipulation -

  ## Managing Data Quality
  ### Circumstances to check for Quality
  - every stop along data life-cycle journey can impact data quality.
 
  ### Automated Validation

  ### Data Quality Dimensions
  - consider multiple attributes of data
  - account for 6 dimensions
    - Data accuracy
    - Data completeness
    - Data consistency
    - Data Timeliness
    - Data Uniqueness
    - Data Validity
   
  ### DQ Rules and metrics
  - understandin data qualuty dimensions, consider how to measure each of them to improve overall quality
  - 

  ### Methods to validate quality
  - Reasonable Expectations
    - check where ot not data in you analytics environment meet reasonable expectations.
   
  - Data profiling
    - use statistical measures to check for data discrepancies, including values that are missing. infrequently ot too frequently occurrence anor ekimination.
   
  - Data Audits
    - use data profiling techniques that help identify data integrity and security issues
   
  - Sampling
    - use a subset of data to inform conclusions about overall data.
   
  - Cross-Validation
    - evaluates how well predictive models perfom
    - divide data into 2
      - training set - build predictive model
      - testing set - determine how accurate the prediction is
    

# Data Analytics and Reporting
- insight is a new piece of information you create from data that influence a decision.
- understand concepts of stats
- learn descriptive stat methods
- inferential stat methods
- types of analysis and key techniques

## Fundamentals of Statistics
- a population represents all the data subjects you want to analyze.
- a census is obtaining data for every element of your population.
- 

</details>

<details>
<summary> Week 2 </summary>
<br>

# Data Analytics and Reporting
## Spreadsheets
- provide intuitive way to organize data into rows and columns.

## Programming Languages
  ### R programming
  - focuses on creating analytics applications.

  ### Python
  - python data analysis library (pandas) provides a set of tools for structuring and analyzing data.

  ### Structured Query Language (SQL)
  - DDL - define structure of database
  - DML - work with data inside a database
  - DDL Commands
    - CREATE - create a new table
    - ALTER - change the structure of a table already created
    - DROP - deletes an entire table from server
  - DML commands
    - SELECT - retrieve information from database
    - INSERT - add new records(Rows) to a database
    - UPDATE - modify rows in the database
    - DELETE - delete rows from a database table

## Statistics Packages
  ### IBM SPSS
  ### Stata
  ### Minitab

## Machine Learning
  ### IBM SPSS Modeler
  ### RapidMiner

## Analytics Suites
  ### IBM Cognos
  - major components
    - Cognos connection - web-based offers access to other elements of cognos suite
    - Query Studio - provides access to data querying and basic reporting tools
    - Report studio - offers advance reporting design tools for complex reporting needs.
    - Analysis Studio - enables advanced modelling and analytics on large datasets\
    - Event studio - provides real time data monitoring and alerting
    - Metric studio - offers the ability to create scorecards
    - Cognos viewer - allows stakeholders to easily interact with data
   
  ### Microsoft Power BI
  - built on SQL server database
  - easy intergration and cost effective
  - major components
    - Power BI desktop - allows to interact with data
    - Power BI is Microsoft (SaaS) offering power BI capabilities in the cloud
    - Mobile apps - provide users of iOS, Android windows device with access to power BI capabilities
    - Power BI report builder - allows developers to create paginated reports
    - Power BI report Server - offers organizations the ability to host their own Power BI environment
   
  ### MicroStrategy
  ### Domo
  ### Datorama
  ### AWS QuickSight
  ### Tableau
  ### Qlik
  ### BusinessOjects

# Data Visualization
## Understanding Business Requirements
- A report is a static electronic or physical document that reflects information at a given point in time.
- Dashboard is an alternative visualization that encourages people to explore data dynamically.
- when developing a report or dashboard understand the auidence and their needs
- after that identify data sources that satisfy their requirments
- pull approach - publish a report to known location eg web page
- push approach - report is automatically sent to appropriate people
- blended approach - (Store the report centrally) inform people that the report is available while maintaining central control of the report itself.

## Inderstanding Report Design Elements
- design principles (5 C's ) of creating visualization
  - Control - how you focus the attention of your auidence
  - Correctness - information mast be accurate with no spelling mistakes
  - Clarity - select right visualization tool for communicating your message and easy to interpret and read
  - Consistency - use same design , documentation elements thoughout
  - Concentration - use visuals to focus auidence attention on rekevant information without overwhelming details.
 
## Report Cover Page
- have a concise title that describes the contents of the report
- communicate a significant insight from the report

## Executive Summary
- provide overview of reports contents
## Design Elements
- color schemes - limited selection of colors use when creating a report / dashboard.
- page layout - determines the arrangement of its component parts.
- font size - 
- style
- charts
- corporate standards
  
## Dashboard Development Methods
- Dashboards are dynamic tools that helps people explore data to inform their decision-making.

  ### Consumer Types
  ### Data Source Considerations
  - static data is data thar refreshes at some regular interval. a design pattern is for operational databases to update a data warehousee everynight.
  - Continuous data (live data) - comes directly from an operational databse that people use to perfom their daily duties. operational database provides live data feed to the dashboard.
 
  ### Data Type Coonsiderations
  - dashboards differs from report as dashboard use software as the delivery mechanism.
  - When creating a dashboard, you use qualitative data to create dimensions.
  - A dimension is attribute used to divide data into categories.
  - a measure is a numeric, quantitative value that a dashboard user is curious about.
  ### Development Process
  - after identify data sources that power your dashboard, develop the dashboard
  - use wireframes - is blueprint for an application that defines the basic design and functions of a dashboard.
  - use mock-up - extends a wireframe by provideing details about visual elements of the dashboard. goal is give a perspective as to the dashboards final user interface.
 
  ### Delivery Considerations
  ### Operational Considerations
  - As you build a dashboard,clearly define the access permissions.
  - Access permissions define the data that a given person can access. 

## Exploring Visualization Types
  ### Charts
  - methods for visualizing both qualitative and quantitative data.
    - Line chart
    - pie chart - presents categorical, or discrete, data as individual slices of the pie.
    - bar chart - presents categorical data.
    - stacked chart -  starts with a bar chart and extends it by incorporating proportional segments on each bar for categorical data.
    - scatter chart -
    - bubble chart -
  - histograms are particularly well suited to illustrating frequency and centrality.
    - is a chart that shows a frequency distribution for numeric data.
  - maps
    - geofraphic maps -
    - heat -
    - tree -
  - warefall - displays the cumulative effect of numeric values over time.
  - infographic -
  - word cloud -  is a visualization that uses shape to signify the importance of words. and eliminate common words and conjunctions.

## Comparing Report  Types
  ### Static and Dynamic
  - static reports pull data from various data sources to reflect data at a specific point in time.
  - Dynamic report give real-time access to information.

  ### Ad hoc
  - Ad hoc reports / one-time use existing data to meet a unique need at a specific point in time.

  ### Self-Service (On-Demand)
  ### Recurring Reports
  - provide summary information on a regularly scheduled basis. get delivered to their audience immediately after creation.
    - Compliance report - detail how your organization meet its compliance obligations.
    - financial compliance
    - safety compliance
    - risk compliance
   
  ### Tactical and Research
  - tactical reports - provides information to onform an organization short term decisions
  - research report helps an organisation make strategic decisions

# Data Governance
## Data Governace concepts
- is set of policies, procesures and controls an organization develops to safeguard its information while making it useful for transactional and analytic purposes.
- it umbrella term covering creation, interpretation and enforcement of data.
- these policies promote data quality, use of data attributes, access to different data domains. also identify how to secure data, comply with regulations, protect data privacy..

  ### Data Governance Roles
- Data stewardship is a=the act of developing the policies and procedures for looking after an organization's data quality, security, privacy and regulatory compliance.
- data steward is responsible for leading an organization's data gorvance activities.
- A data owner is a senior business leader with overall responsibility for a specific data domain.
- A data domain/ data subject area contains data about a particular operational division within organization.
- subject area data steward works in the data owners organization.
- a data custodian is a role given to someone who implements technical controls that execute data governance policies. usualky IT who configure applications, dashboards and database.
- Data access requirements determine which people need access to what data.
- when determining access requirements, essential to develop data classification matrix.
- Data classification matrix defines categories, descriptions and disclosure implications for data
- A data steward works with a data owner to establish broad classifications, with subject area data stewards to develop procedures for granting access to information, and with data custodians to ensure the appropriate technical controls are in place to protect information.

  ### Access Permissions
  - Role-based acess means that instead of giving access to individual people, you grant access to the role they occupy.
  - a role-based access approach facilitates permissions maintenance and improves consistency.
 
  ### Group Permissions
  - an organization chart documents the reporting structure within an organization.
 
  ### Data Use Agreements
  - A data use agreement (DUA) is a conctractual document for transferring private data between organizations. establish a dua before sharing data with outside party.
 
  ### Security requirements
  - TECHNICAL CONTROLS FOR PROTECTING DATA.
  - Data encryption for data protection, as data is unsuable without the key to decrypt it.
  - Encrypt data at rest as well as data in trnasit to keep it secure.
  - data at rest locations is databases and flat files.
  - Transparent Data Encryption (TDE) ensure the database files and log file are encryped.
  - data ib transit is data actively moving between one location to another, during data transmission encrypt the connection between the locations.
  - transmitting data over internrt uses HTTP to ensure data security use TLS.
 
  ### Storage Environment Requirements
  - data at rest exist in local storage, shared drive and cloud, regardless of storage environment encrypt all data at rest.
 
  ### User Requirements
  - specify how to collect, process, use, store, retain and remove data.
  - crucial to effective data govarnance
  - An acceptable use policy (AUP) defines an individual's responsibilities when accessing, using, sharing and removing organizational data.
  - AUP has provisions for each type of data in an organizations's data classification matrix.
  - AUPs describe acceptable locations for storing proprietary information; what to do in the event of theft, loss, or unauthorized disclosure; and methods of disposal.
 
  ### Entity Relationship Requirements
  - 

  ### Data classification requirements
  - is the process of analyzing data and organizing it into risk-based categories.
</details>
