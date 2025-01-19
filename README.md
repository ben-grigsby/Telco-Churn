Telco Customer Churn Analysis
Overview.
	This project analyzes customer churn data for a telecommunications company,  identifying the key drivers behind customer churn and providing actionable insights to reduce churn rates. Various machine learning techniques, including Random Forests and hyper-parameter tuning, were employed to maximize the model’s predictive performance.

Dataset.
	The dataset was a slightly altered version of the IBM Telco Customer dataset. Alterations mainly included the removal of specific locations of customers, the longitude and latitude. The dataset consisted of 7043 observations alongside 21 parameters. A brief description of a couple of the features include, ‘Tenure’ which describes how long a customer has been subscribed to the company, ‘Subscription’ which describes the type of contract a customer has with the company, and ‘Churn’ which describes the churn status of a customer. 

Objectives.
	The main objectives of this analysis was to analyze patterns in customer churn, build predictive models to classify customers into churners and non-churners, use those models to tell us what features are important when it comes to predicting customer churn, and what actionable insights we can take moving forward now that we know what features contribute most to churn rate. 

Methodology.
1.	Exploratory Data Analysis (EDA)
  a.	Visualizations of churn rates by tenure, and monthly cost, amongst other features 
  b.	Handling missing values and data transformations
2.	Model Building 
  a.	Initial Random Forest Model 
  b.	Implementation of class balancing (e.g. ‘class_weight=balanced’)
  c.	Resampling of data using SMOTE 
  d.	Hyperparameter tuning using GridSearchCV
  e.	Evaluation metrics like accuracy, recall, precision, F1-score, and ROC-AUC
3.	Feature Importance Analysis
  a.	Identification of the most influential features 
  b.	Insights and recommendations based on feature importance


Key Findings.
1.	Churn is highly influenced by factors like tenure, total charges, and subscription type 
2.	Longer-tenured customers are less likely to churn 
3.	Customers on a two-year contract are less likely to churn 
4.	Customers spending more on a subscription package are less likely to churn 
5.	A rewards program target early-tenure customers may help reduce churn 

How To Run The Code.
1. Clone the repository
   a. Start by cloning the repository to your local machine:
       git clone https://github.com/ben-grigsby/Telco-Churn.git
       cd project-repo-name
2. Set up the environment
   a. Install Python: Ensure Python (preferably 3.12.2, or higher) is installed on your machine. You can download it from https://www.python.org/
   b. Install required libraries: use the requirements.txt file provided in the repository:
       pip install -r requirements.txt
3. Prepare the dataset
   a. The initial dataset for this project is in the repository titled, 'customer_data.csv'
4. Launch Jupyter Notebook
   a. Open Jupyter Notebook from your terminal or command line:
       jupyter notebook
   b. Navigate to the final_report.ipynb notebook file and open it

Future Work.
1.	Explore Advanced Algorithms
  a.	Implement XGBoost to evaluate its performance compared to Random Forest in predicting churn 
2.	Simulations for Rewards Program
  a.	Design and run simulations with realistic pricing models to test the effectiveness of the proposed rewards program 
  b.	Continuously iterate and refine the program based on simulation results 
3.	Natural Language Processing (NLP)
  a.	If customer feedback or reviews are available, use NLP techniques to analyze text data
  b.	Identify factors that influence customer retention and churn by extracting insights from customer sentiment and complaints 
4.	Incorporate More Data Sources
  a.	Leverage external data (e.g. economic indicators, competitor analysis) to enhance model robustness and gain a more comprehensive understanding of churn drivers 
5.	Dynamic Feedback System
  a.	Build a pipeline to incorporate customer churn data dynamically and adjust predictions and insights over time 


