# spark-mllib-deployment
Pyspark MLlib model deployment

## Project Outcomes 

Project involves the following objectives:
1. Creation of a Regression model using Pyspark MLlib library
2. Creating a pipeline in Pyspark
3. Save the Load the model using MLFLow
4. Serve the model using MLFlow 


## Dataset 
Boston Housing Dataset

## Resources 

Used the wrapper from "https://github.com/amesar/mlflow-tools" due to the error from the Pyspark 

 ************ PROBLEM *************
 Currently you cannot load a SparkML model as a UDF with MLflow due to named column bug.
 Error message: pyspark.sql.utils.IllegalArgumentException: CRIM does not exist. Available: 0, 1, 2, 3
 mlflow git issue 4131 - Spark UDF throws IllegalArgumentException

 ***********  SOLUTION **************
 There is a workaround that leverages a custom PythonModel wrapper.
 Wrapper: sparkml_udf_workaround.py
 Usage: test_sparkml_udf_workaround.py





