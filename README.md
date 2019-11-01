## Neo3 explorer lambda/dynamodb deployment notes

### Initial deployment
```
serverless deploy -c serverless-initial.yml
```
### Subsequent deployment (for updates to the API)
```
serverless deploy -c serverless-update.yml
```

AWS IAM role for DynamoDB and Lambda functions is required - 
either use ~/.aws/credentials file with IAM API key or assign
the appropriate IAM roles to the EC2 instance where the API
will be deployed from (preferred method)
