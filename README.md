# 

```bash
 
To prepare the application for deployment, use the `sam package` command. 
To deploy the application, use the `sam deploy` command. 

```
 
```bash

sam package  --output-template-file packaged.yaml  --s3-bucket vashi-lambda-code
sam deploy --template-file packaged.yaml --stack-name LambdaDependentCodeLayer --capabilities CAPABILITY_IAM

```
 
