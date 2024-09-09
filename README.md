# MLFLOW-Basic_Operations

import dagshub
dagshub.init(repo_owner='JeevanBiju', repo_name='MLFLOW-Basic_Operations', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)


  MLFLOW_TRACKING_URI = https://dagshub.com/JeevanBiju/MLFLOW-Basic_Operations.mlflow
  MLFLOW_TRACKING_USERNAME = JeevanBiju
  MLFLOW_TRACKING_PASSWORD = c601a9b872def1de041303581619277de227361a



 sudo apt update
 sudo apt install python3-pip
 sudo pip3 install pipenv
 sudo pip3 install virtualenv
 mkdir mlflow
 cd mlflow
 pipenv install mlflow
 pipenv install awscli
 pipenv install boto3
 pipenv shell
 aws configure
 mlflow server -h 0.0.0.0 --default-artifact-root s3://mlflowbuc1
 
export MLFLOW_TRACKING_URI = http://ec2-54-173-17-44.compute-1.amazonaws.com:5000/