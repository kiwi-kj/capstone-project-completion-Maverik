# Time-Series Analysis for Maverik
Group Project for IS 6813-001 - Fall 2023
### Team Data Dive_rse
Che, Kalyani, Debayan, Disha

- - - - 

## Table of Contents

1. [Business Problem Statement](#business-problem-statement)
2. [Project Objective](#project-objective)
3. [Analysis and Implementation](#analysis-and-implementation)
   - [Data Analysis](#data-analysis)
   - [Feature Engineering](#feature-engineering)
   - [Building Model and Validation](#building-model-and-validation)
   - [Business Impact](#business-impact)
   - [Continual Improvement](#continual-improvement)
4. [Group's Solution](#groups-solution)
5. [Contribution](#contribution)
6. [Business Value](#business-value)
7. [Difficulties Encountered](#difficulties-encountered)
8. [Learning](#learning)

## Business Problem Statement <a name="business-problem-statement"></a>
Maverik is embarking on an annual expansion initiative, planning to open 30 new stores, and needs a precise predictive model for first-year sales to support financial planning and ROI calculations. The ability to make well-informed decisions regarding store locations and resource allocation, coupled with achieving specific sales targets and monitoring progress, hinges on the accuracy of these forecasts. The success criteria for the proposed solution involve generating forecasts within a 10% accuracy range, adaptability to new data, and a user-friendly interface. Leveraging machine learning techniques, we will initiate the creation of a forecasting model by conducting thorough data analysis and training various models using historical sales data. The project's scope encompasses developing an R-based model capable of daily-level sales forecasts, including annual projections while accommodating seasonality and the ability to update forecasts with new data. This project is executed by the Data Dive_rse team, utilizing R for model development. The project concluded in December 2023, with milestones including in-depth exploratory data analysis, model building, and comprehensive model evaluation.

## Project Objective <a name="project-objective"></a>
Maverik is interested in producing more accurate financial plans and initial ROI documents for future convenience store locations. The goal of this project is to develop a predictive model that is precise enough to forecast the first-year sales of new stores that Maverik plans to open. This predictive model will be an ensemble of forecasting and supervised regression models designed to provide daily store-level sales forecasts of multiple key metrics viz "inside sales", "food service sales", "diesel sales" and "unleaded sales" which will aid Maverik in financial planning, resource allocation, and ROI calculations for its expansion strategy. The Success of this project will be benchmarked against Maverik’s existing Naive forecasting solution. The ability to accurately forecast store sales will enable Maverik to optimize the expenditure of scarce resources by pursuing the most profitable locations and minimizing the misallocation of said resources when opening a new store. This will lead to better investment, decreased waste, and more reliable financial evaluations.

## Analysis and Implementation <a name="analysis-and-implementation"></a>

### Data Analysis <a name="data-analysis"></a>
- Conducted in-depth analysis of 38 stores, and the qualitative dataset with 37 records and 55 features.
- Conducted in-depth analysis of the time series dataset with 13908 records and 12 features.
- Focused on exploring various sales metrics such as "inside sales", "food service sales", "diesel sales" and "unleaded sales" across store open year, daily sales date, week ids & various services provided by the store.
- Examined the dataset for missing values and identified that there are six columns in qualitative dataset with missing values.
- Provided valuable insights for data pre-processing and modeling decisions.

### Feature Engineering <a name="feature-engineering"></a>
- Prepared data for modeling by removing redundant columns and columns with no variance.
- Replaced missing values in the qualitative dataset with "unavailable" as N/A here means not available(meaning that a specific service is not available for that store).
- Examined the trends and seasonality patterns in each sales metric by visualizing their relationship with the date through ggplot plots.

### Building Model and Validation <a name="building-model-and-validation"></a>
- Implemented Vector AutoRegressive Model (VAR) on time series data.
- Evaluated model performance using metrics such as MAE, RMSE, MSE for each sales metrics.
- Compared VAR model with other models to assess relative performance.

### Business Impact <a name="business-impact"></a>
- Emphasized potential business impact, especially in terms of future forecast for each sales metrics.
- Highlighted the model's role in fostering financial planning and increase ROI by forecasting sales for each store by EoY.

### Continual Improvement <a name="continual-improvement"></a>
- Designed the model with scalability and adaptability to accommodate future data updates and evolving business needs.
- Recognized the importance of ongoing model enhancement and optimization.

## Group's Solution to the Business Problem <a name="groups-solution"></a>
Our group implemented various models, to forecast future sales and see which model performs the best. The model's performance was rigorously evaluated using metrics such as MAE, RMSE, and MSE. Our collaborative efforts and problem-solving skills resulted in a robust solution that Maverik can leverage to forecast year long sales for new stores which in turn can help them in making strategic decisions and financial growth.

## Contribution <a name="contribution"></a>
As a team member, I actively participated in various aspects of the project. Played a crucial role in conducting in-depth data analysis, exploring the key sales metrics, identifying trends and seasonility, and providing valuable insights for data pre-processing and modeling decisions. Additionally, I prepared the data for VAR model and implemented the model to forecast sales for each key metrics. 

## Business Value of the Solution <a name="business-value"></a>
The successful implementation of our model has immense business value for Maverik. By accurately forecasting sales, Maverik can make more informed strategic decisions, reducing waste, and increasing profitability. Precise forecasts will enable them to make informed decisions on store locations and resource allocation along with achieving set sales targets while checking the progress.

## Difficulties Encountered <a name="difficulties-encountered"></a>
Throughout the project, our team encountered challenges related to handling multi-variate, multi-target time series data. Provided data was just for one year which was not enough to accurately forecast total sales. However, our collaborative efforts and problem-solving skills enabled us to overcome these difficulties and deliver a robust solution.

## Learning <a name="learning"></a>
Through this project, I have gained invaluable experience in data analysis, feature engineering, for multi variate/targeted time series forecasting. I learned how to interpret time series model results and communicate insights effectively. Additionally, working in a team setting enhanced my collaboration and communication skills, contributing to a successful outcome.

In conclusion, our Maverik time series forecasting project showcases our dedication to data science, collaboration, and delivering business value. It is a testament to our problem-solving abilities and highlights the impact of data analysis in driving informed decisions for Maverik and fostering financial planning.
