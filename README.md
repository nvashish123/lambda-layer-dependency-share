# 

```bash
 
To prepare the application for deployment, use the `sam package` command. 
To deploy the application, use the `sam deploy` command. 

```
 
```bash

Layers:
- !Sub arn:aws:lambda:us-east-1:905621505184:layer:BotoLayer:2

sam package  --output-template-file packaged.yaml  --s3-bucket vashi-lambda-code
sam deploy --template-file packaged.yaml --stack-name LambdaDependentCodeLayer --capabilities CAPABILITY_IAM

```
 
