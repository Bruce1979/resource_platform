# Data Science resources, activities and tools

A high level overview of the topics explored across the 4 units of the Data Science course:

* Data representation
* Data analysis tools and techniques
* Spreadsheets
* Databases
* Data visualisation tools and techniques
* Big data
* Open data and APIs
* Machine learning

# General Data Science Resources

The following resources are useful to develop your own understanding of Data Science, and include many activities and resources that can be used/adapted in various units in the Data Science course:

[Ranked Intro to Data Science courses](https://www.freecodecamp.org/news/i-ranked-all-the-best-data-science-intro-courses-based-on-thousands-of-data-points-db5dc7e3eb8e/)

# Unit One: Data Representation and Analysis

## Concepts overview:

### What is Data?
* What is the history of Data?
  * DIKW pyramid
* What can data tell us?
* Why is this interesting?
* Looking at data, analysis and representation (visualisation)
  * Tell amazing stories using data
* Ethics of data

### Where do we get Data from?
* Data about people - collected from forms
* Environmental data - from the world directly (e.g. sensors)
* Data from actions (web browsing data) and inference
* Metadata - what is it?
* Arduino / Microbit programming - sensor data collection, transfer, storage
* Varieties of data
* Consider data collection issues:
  * Privacy and security
  * Legal considerations
  * Sustainability
  * Ethics
  * Bias/Distortions
  * Data Quality
* Availability of data:
  * [ACT Open Data Portal](https://www.data.act.gov.au/)

### How do we understand the limits of data?
* What can and cannot be represented by data?
* How “complete” is your data? What is missing? When is it complete enough?

### How do we model/represent data?
* Choices made in representation and collection can affect outcomes
* Modelling objects vs. events vs. relationships
* Quantitative vs qualitative
* What choices might be made in representing a quantity?

### How do we analyse data?
* Grouping
* Sorting
* Filtering
* Aggregation
* Summarisation
* Trend and pattern analysis
* Tools
  * Spreadsheets
  * Pandas / Numpy / Matplotlib / programming
* Correlation vs causation vs coincidence
  * Spurious correlations
* Consider data analysis issues:
  * Ethics
  * Bias/Distortions
  * Using data for decision-making (Centrelink?)

### How do we present data?
* Graphs - types, suitability, choices
* Summary statistics (compare suitability using Anscombe's quartet)
* Tables
* Animations (stretch goal) / interactive representations
* Looking at different visualisations 
  * [US Gun Deaths](https://guns.periscopic.com/?year=2013)
  * [Google Public Data - Life Expectancy vs Fertility Rate](https://www.google.com/publicdata/explore?ds=d5bncppjof8f9_&ctype=b&strail=false&nselm=s&met_x=sp_dyn_le00_in&scale_x=lin&ind_x=false&met_y=sp_dyn_tfrt_in&scale_y=lin&ind_y=false&met_s=sp_pop_totl&scale_s=lin&ind_s=false&dimp_c=country:region&ifdim=country&iconSize=0.5&uniSize=0.035)
  * [Worldometers - Real time data](https://www.worldometers.info/)
* Abuses of presentation
  * inconsistent scales
* Develop narratives (through presentations)


## Program of learning

|Week|Module|Length|Title|Description|
|--|--|--|--|--|
|1|1|2 hours|Amazing stories|Introduce students to data through visualisation and narrative|
|2|2|4 hours|The history and nature of data|What is Data Science? What is Data? Why does it matter? Introduce ethical issues (Data distortions and bad decision-making)|
|3 - 4|3|8 hours|Data Representation|What is data representation? Modeling the world as discrete values (e.g. numbers, enum) Data types etc. (includes intro programming - csv manipulation, data types in programming languages, binary reps)|
|5 - 6|4|8 hours|Exploring datasets|Spreadsheets, Online / visualisation tools, Data quality, Interpretation, Visualisation|
|7-8||8 hours|Assignment, Review, Exam||
|9 - 10|5|8 hours|Analysing and Visualising Data||
|11 - 12|6|8 hours|Programming Techniques for Analysis and Presentation||
|13|7|4 hours|Project: Designing a data collection|Modelling data|
|14-16|8|8 hours|Major Project: Constructing, analysing and presenting data||
|17-20|12||Review, Exam, Assessment & Reporting||

## Resources and case studies

TODO

# Unit Two: Big Data Analysis and Techniques

## Concepts overview:

### What makes data "big"? How is it different from data?
* How is big data represented?
* Where is it stored?
* How does it travel?
* 4 Vs of big data:
  * Volume
  * Velocity
  * Variety
  * Veracity

### What are the issues raised by Big Data?
* Ethical issues
* Privacy
* Security
* Storage Requirements
* Sustainability
* Decision-making systems

### If Big Data is the tool, what is the problem?
* Problems solvable using big data
* Why is big data required?

### Big Data Algorithms
* Need for Parallelism (too large for a single machine/cpu)
* Functional Programming Paradigms - suited to parallelism
* **MapReduce**
  * the key algorithm for dealing with big data
  * maps a function to a dataset
  * reduce collects the results of the function application to the dataset
  * key algorithm behind the success of Google's pagerank 
  * for Sorting large datasets - the algorithm used to sort must be parallelisable (MergeSort, Odd-Even Sort, Non-Comparison Sorts)


* **Random Sampling**
  * If your application relates to a statistical analysis - random sampling helps reduce the size of your data problem
  * Traditional sampling methods can be used
  * How big / small does a sample have to be to derive meaningful conclusions?

* **Variety**
  * Multivariate Algorithms
  * Feature Extraction
  * Clustering

* **Volume**
  * MapReduce (using PyDoop interface to Hadoop and Hadoop Distributed File System
  * Filtering / Selection

* **Velocity**
  * Dynamic Algorithms

* **Veracity**
  * How do you check if data is true and meaningful?
  * Is it valid to filter out unexpected or unwanted data?
  * For example: extracting data from Twitter that is not generated by bots / is generated by bots

### Big Data Tools (Python)
* PyDoop - Python interface to Apache Hadoop for access to MapReduce and HDFS
* PySpark - Python interface to Apache Spark for access to RDD (Resilient Distributed Datasets)
* NetCDF4 - Python implementation to netCDF, which enables OPeNDAP distributed datasets (including NCI hosted datasets)
* Xarray - Handles netCDF4 data connections to read data into python

### Big Data Management
* Connectivity, APIs, (cannot take all the data at once, cannot store it locally)
* Structured storage & APIs (databases) (Volume)
* SQL and NoSQL (Variety)
* XML & JSON
* Summarisation and filtering (Velocity)

### Big Data Analysis
* Trend Analysis
* Cluster Analysis
* MapReduce
* Slicing, Dicing, etc.

### Big Data Visualisation
* look at geospatial data and mapping
* animations
* interactions

### Big Data and Decision Making
* how to make a decision based on your analysis
* good decisions vs bad decisions
* Coincidence correlation causation

### Telling stories with big data
* Applying Big Data techniques to new data sets; building narratives and uncovering stories.

## Program of learning

|Week|Module|Length|Title|Description|
|--|--|--|--|--|
| 1 | 1 | 3 hours | Intro to Big Data Analytics | What is Big Data and why is it important? |
| 2 | 2 | 4 hours | Types of Big Data | Volume, Velocity, Variety, Veracity. Where do we find big data?  Assess the data input into a human from all senses/sensors - how much data is this? Practical - Python refresher/intro + Finding and locating big data |
| 3 | 3 | 4 hours | Issues with Big Data | **See above for details** Suggested Practical == Passing a function as a parameter in Python |
| 4-5 | 4 | 8 hours | Algorithms == MapReduce | Explore how to use this core algorithm, and how to implement it in Python. Practical == MapReduce |
| 6 | 5 | 4 hours | Tools == PyDoop | Using Hadoop through PyDoop to implement MapReduce on a large dataset |
| 7 | 6 | 4 hours | Managing Big Data | APIs, Connectivity, Data Formats, Query Languages |
| 8 | | 4 hours | Revision + Test | |
| 9-10 | 4 | 8 hours | Algorithms Revisited | Choose several from Clustering, Multivariate Analysis, Feature extraction, Filtering, Sampling |
| Break | | 2 weeks | | |
| 11-12 | 7 | 8 hours | Big Data Analysis | Applying algorithms to problem domains |
| 13 | 8 | 4 hours | Big Data Visualisation | Example: Geospatial data representation / other selected visualisation technique |
| 14 | 9 | 4 hours | Big Data and Decision-Making | Look at examples of bad decision-making (robo-debt) and good decision-making. What makes for good and bad decisions? Can you make good decisions with bad data? Or bad analysis? |
| 15-16 | | 8 hours | Student Projects | Help students find data, select data, choose appropriate analytical techniques, and create visualisations | 



## Resources and case studies

TODO

# Unit Three: Machine Learning (ML)

## Concepts overview

### Social and Environment Impacts of ML
Machine learning is a powerful technique which enables computers
to 
* recognise patterns in data
* identify objects within images or from sounds
* predict outcomes/future pathways based on prior "experience"
* make recommendations based on observed behavioural patterns
* generate new content from models built from "learned" data

ML technology promises great benefits in improvements in system capability, user interactions, customised and curated experiences, speed of business processes and expansion of services offered to citizens and consumers - even to learners! 

These capabilities were previously the domain of human endeavour, in an industrial context. As ML capabilities develop, more "human-labour" employment tasks can be transferred to ML-backed systems.

The social impacts of this transformation are immense: 
* transformation of labour and work
* social control through extensive or universal monitoring (panopticon)
* social control through ML curated lived experiences -  
ML systems will know individuals preferences so well, nudging or driving consumer purchasing/electoral/life decisions in the directions chosen by organisations or government
* social control through predictive policing / social credit systems
* will ML-backed systems replace human capability?    
why would a human learn to do "x" if the computer can do it better -     
where "x" moves from "navigate a map" to "write an essay" to ???

The environmental impacts of ML will be driven by scale in a number of ways:
* how many systems can transform into ML-backed systems?
* what are the resource needs of these systems?
* how much energy does it take to train a large ML system    
(such as image recognition)?
* what are the networking requirements of ML systems -     
is edge computer sufficient, or are we sending images over a network to a server for recognition?
* how long before the next technology upgrade cycle?  
* how much waste is generated?

### Legal and Ethical Aspects of ML
As our systems move to ML-capability, what are the legal restrictions we will need to put in place to ensure individuals, governments and companies are protected in terms of:
* privacy and security - including identity
* choice of engagement (opting in and opting out)
* intellectual property
* right to work
* right to presumption of innocence
* right to freedom from discrimination of any kind     
(bias in data creating bias in outcomes - which are applied to automated decision-making)
* right to a sustainable future
* equity of access to technology and its benefits -     
a more equitable distribution of access to "future tech".

### ML Approaches and Models
#### Aproaches
The main approaches to Machine Learning [as at 2020] are:
* Supervised Learning:    
  all training data is labelled with categories. The ML system established the boundaries for identifying different patterns based upon the labels provided
* Unsupervised Learning:    
  training data is not pre-categorised. Massive training datasets are used with different algorithms which assist in separating data into discrete groups (clustering). The groups can be used for subsequent pattern recognition without human operator intervention. This can be used for anomaly detection, associations, or auto-encoding
* Reinforcement Learning:    
  In reinforcement learning, a system of "high-value goals" are used to reinforce successful achievement, promoting the capability of a system. This has been used to develop game-playing agents which can outperform than human agents. Reinforcement learning can be used in any system which has discrete steps, and in which the value of a step, or outcome, can be classified.
* Semi-supervised learning    
  is a combination of supervised and unsupervised learning approaches.     
  It is not expected that teachers would cover semi-supervised learning.

#### Models
In this context a model is taken to mean the data structures and associated computational components which have been trained using a set of data, validated using a set of data, and can then be used to make predictions based on final input data.

The "shape" of a model is dependent upon the algorithms and approach chosen for the selected problem domain. Models built using Artifical Neural Networks wil have a different shape and size to those built using Linear Regression, to those using k-Means Clustering, to those using Reinforcement Learning.

It is also crucial to cover the selection of an ML approach/model for a given problem. Which problems can be solved using an ML approach, and which cannot be solved using an ML approach. 

### Data Preparation Requirements for ML
Part of the beauty of Machine Learning is that it can be trained on unstructured data, or less structured data. Attempting to analyse a photograph without using machine learning, based on the numeric values of pixels is extremely challenging. Recognising objects in pictures is almost impossible without ML.

The challenges for building robust systems of machine learning are of obtaining high-quality labelled data to suit your ML application. Often data labels must be added by domain experts.

For image recognition, conditions such as lighting, white balance, focus, aperture effects, blur affect imaage quality: this apples to both training data, and data used for image recognition. Ensuring that systems have sufficient "exposure" to the range of possible conditions is critical to ensuring a successful image recognition system.

Diversity of input is critical to ensuring that your system avoids systemic bias and failure of service delivery. For example: in a voice recognition system, in order to recognise every accent of a language, an ML system requires exposure to EVERY accent, with labelled data.  It should not require exposure to every voice. 

* Data selection:     
  selecting the correct data for your ML problem: data must be relevant, high quality, requisite features are present in the data. Data
  selection must retain the diversity necessary to meet the problem domain
requirements.
* Data cleaning:     
  checking your data is consistent, no missing data
* Labelling:     
  all data is labelled (supervised, semi-supervised, reinforcement)
  Labels are correct and identify requisite features
* Formatting:    
  data must be formatted so that it is consistent (e.g. images for recognition must be in a consistent resolution). Downsampling may be a useful strategy - as it will also improve training speed and recognition speed.

### ML Algorithms
The wide range of ML algorithms meet different problem domain requirements in different ways. Algorithm selection should be guided by experience, the training data available, and the desired shape of a problem solution. 

Decision points may include:
* Is your input data labelled into discrete categories?
  - implies supervised learning models
* Do you want to separate a set of data into discrete groups?
  - implies unsupervised learning models
* Are you looking to optimise the performance of a system based on defined goals?
  - implies reinforcement learning models
* Is the output of your problem a binary decision 
  (member of category X, or not member of category X)?
  - classification algorithms
* Is the output of your problem a numeric value?  (the probability of a recommendation being useful)?
  - regression algorithms
* Is the output of your problem a set of groups?
* How much compute time is reasonable to find a solution?  
  - How time efficient does your system need to be when deployed?
  - How much time is required to build, train and test the model?
* How accurate does your solution need to be?
* What level of expertise is required to interpret a given solution?
* What is the complexity of the data model?
* How scalable do you need the solution to be?

This ML cheatsheet from SAS (Hui Li) is a useful guide to algorithm selection:
![ML Cheatsheet](https://blogs.sas.com/content/subconsciousmusings/files/2017/04/machine-learning-cheet-sheet-2.png)

Microsoft also publish a useful ML algorithm selection cheetsheet:
![MS Azure ML Cheatsheet](https://docs.microsoft.com/en-us/azure/machine-learning/media/algorithm-cheat-sheet/machine-learning-algorithm-cheat-sheet.svg)

### ML Outputs
* Recognition
  - the main subject of an image
  - individual objects that are contained in an image (automatic tagging)
  - anomalies and "hidden features" within images - assisting with diagnosis
  - words, phrases, or statements are contained within an audio sample
  - what features are present within an audio sample
  - fraud detection (anomalies in transaction)
  - spam detection
  - phishing detection
* Prediction
  - predicting numeric values in a range
  - predicting between membership of 2 or more categories
  - predicting flows (traffic, financial, network)
  - dynamic pricing
  - cyber threat detection

* Recommendation
  - predicting what a system user may be interested in, or what a consumer may be interested in purchasing 
  - recommending the next move in a game
  - customising search engine results per user
* Generative
  - generating output as generative art (visual, audio, video, 3D models, etc.)
  - generating text in response to input prompts - replacing expert systems - chatbots, customer support, etc.
  - language translation
  - deep fakes
  - custom video backgrounds

### ML Visualisation
ML can be used to generate visualisations for data analytics. Outputs include 
linear regression, category membership with probability of correct classification, clusters within data, etc.

Understanding what is happening within a complex ML system when it makes predictions or recommendations, or recognition, is vital to ensuring that outputs meet community ethical, moral and legal standards: explainability is key to acceptance. [Much has been written](https://medium.com/@shagunm1210/the-explainable-neural-network-8f95256dcddb), but this is an area for further development.

### Bias in data and impact upon ML
There are multiple issues with bias in machine learning:
* Selection of training data: As an example - using only male voices from 
limited demographic samples in your training set will lead to voice recognition failing on any unrepresented accent or tonal pattern; using only faces from a white community in your training data can lead to non-white faces being recognised at all, or miscategorised as non-human.
* Unintentional systemic bias: our societies are rootedin multiple, integrated systems of power, and of oppresion.  As individuals brought up within a system, we adhere to the social norms, often without questioning the basis for the norms (is the accumulation of staus, wealth, power in the hands of the few ideal; is greed a natrual human trait)? Our ML systems will replicate and amlify systemic bias if not addressed during design.  [More here](https://towardsdatascience.com/bias-what-it-means-in-the-big-data-world-6e64893e92a1)
* Intentional bias: predictive policing and the use of ML-enabled decision making in legal cases, or recruiting employees, intentionally reinforces systemic bias. This can lead to an amplification of bias. [Hello World by Hannah Fry](https://www.penguin.com.au/books/hello-world-9781784163068) covers multiple cases of intentional bias. [Read More](https://www.versobooks.com/books/3002-new-dark-age)     


## Program of learning

|Week|Module|Length|Title|Description|
|--|--|--|--|--|
|1|1|2 hours|Wow - ML in Practice|Introduce students to Machine Learning through demonstrations and narrative|
|2|2|4 hours|ML Overview|What is Machine Learning? ML Approaches and Models. Introduction to ML Algorithms. Social and Environment Impacts of ML.|
|3 - 4|3|8 hours|Using ML systems|ML data input preparation requirements. ML Outputs. What are the implications of using ML to solve a problem? Legal and ethical issues of ML. Bias in data and impact upon ML.|
|5 - 6|4|8 hours|Algorithms: Regression|Using multi-variable linear regression as Machine Learning. Selecting regrtession as a solution - limitations and benefits. Determining which problems are suited to multi-variable regression.|
|7-8||8 hours|Assignment, Review, Exam||
|9 - 10|5|8 hours|Algorithms and Models: Supervised Learning using SVM|Naïve Bayes and/or linear Support Vector Machines, for classification of large data sets|
|11 - 12|6|8 hours|Algorithms and Models: Supervised Learning using ANN|The perceptron algorithm. Types of Neural Networks. Compute and time requirements for training large Neural Networks. Transfer Learning. Deep Learning|
|13|7|4 hours|Algorithms and Models: Unsupervised Learning|k-Means Clustering (numerical data), or k-Modes Clustering (categorical data)|
|14-16|8|8 hours|Major Project|Constructing an ML application, training and validating a model, analysing outputs, and presenting findings|
|17-20|||Review, Exam, Assessment & Reporting||

## Resources and case studies

ImageNet Roulette
