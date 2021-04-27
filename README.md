# Udacity-Capstone-Starbucks-challenge
Contains all the files used during the Udacity Capstone Starbucks challenge
Table of Contents
1.	Project overview
2.	Components
3.	Installation
4.	File Descriptions 
5.	Instructions
6.	Thanks, Acknowledgements and references

1. Project Overview
Starbucks provided simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. Not all users receive the same offer, and that is the challenge to solve with this data set. 
2. Project Components
This is the Starbuck's Capstone Challenge of the Data Scientist Nanodegree in Udacity. We get the dataset from the program that creates the data simulates how people make purchasing decisions and how those decisions are influenced by promotional offers. 
We are interested to solve the following question:
1.	Which offer(s) should be sent to a particular customer:
The main steps that are followed:
•	We make initial exploration of the data and perform cleaning pre-processing to be ready to be used by an algorithm.
•	We perform a quick Exploratory Data Analysis (EDA) to have some insight into the data.
•	We will fit Funk SVD with the specified hyper parameters to the data.
•	We perform evaluation and validation using mean squared error for latent features of 5, 10, 15 and 20.
•	Finally, we create a recommendation of which Starbucks offers should be sent to a particular user as well as recommendation to a new user.
3. Installation
•	The code should run with no issues using Python versions 3.*.
•	No extra besides the built-in libraries from Anaconda needed to run this project
•	Data Processing & Machine Learning Libraries: NumPy, Pandas, Sciki-Learn
•	Data Visualization: Matplotlib, Seaborn
4. File Descriptions
The data is contained in three files:
•	portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
•	profile.json - demographic data for each customer
•	transcript.json - records for transactions, offers received, offers viewed, and offers completed
•	user_item_matrix.p – user-item matrix that can be used instead of waiting for the creation of this file to be completed
•	test_df.p – test_df data file that can be used instead of waiting for the creation of this file to be completed
•	train_df.p– train_df data file that can be used instead of waiting for the creation of this file to be completed
Here is the schema and explanation of each variable in the .json files:
portfolio.json
•	id (string) - offer id
•	offer_type (string) - type of offer ie BOGO, discount, informational
•	difficulty (int) - minimum required spend to complete an offer
•	reward (int) - reward given for completing an offer
•	duration (int) - time for offer to be open, in days
•	channels (list of strings)
profile.json
•	age (int) - age of the customer
•	became_member_on (int) - date when customer created an app account
•	gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
•	id (str) - customer id
•	income (float) - customer's income
transcript.json
•	event (str) - record description (ie transaction, offer received, offer viewed, etc.)
•	person (str) - customer id
•	time (int) - time in hours since start of test. The data begins at time t=0
•	value - (dict of strings) - either an offer id or transaction amount depending on the record
5. Instructions
1.	The analysis is contained within the Jupyter notebook.
2.	 3 json files should be located in data folder.
3.	Use the pickle files to avoid waiting for the process to run
6. Thanks, Acknowledgements and references 
Starbucks for the data
Udacity for the course and support
https://www.researchgate.net/post/How-do-I-measure-the-robustness-of-a-ML-model-against-adversarial-samples
https://towardsdatascience.com/metrics-to-evaluate-your-machine-learning-algorithm-f10ba6e38234
https://stackoverflow.com/questions
Reddit learnpython community
Fellow Udacity students
Colleagues
Family
7. Results
The main observations of the code are published on medium https://jaco-vanderwalt.medium.com/how-to-use-funk-svd-to-recommend-an-offer-a-learning-journey-of-discovery-1b45f7007e52
