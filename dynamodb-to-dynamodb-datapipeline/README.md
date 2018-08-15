# dynamodb-to-dynamodb-datapipeline

Data pipeline that copies DynamoDB source table to DynamoDB destination table using S3 bucket as a temporal storage

To deploy using aws cli:
```sh
aws cloudformation deploy \
  --template-file template.yml \
  --stack-name dynamodb-to-dynamodb-datapipeline \
  --parameter-overrides SourceTableName=<source-table-name> DestinationTableName=<destination-table-name> \
  --template datapipeline-template.yml \
  --profile cloud-formation@flowlab-development
```

Template has been created based on [https://github.com/aws-samples/data-pipeline-samples](https://github.com/aws-samples/data-pipeline-samples)

In case of error: 
> Pipeline Definition failed to validate because of following Errors: [{ObjectId = 'NameEmrCluster', errors = 
[Invalid role 'DataPipelineDefaultRole' in slot 'role'. Please make sure that the role exist and Data Pipeline 
has permission to assume the role.

deploy [role template](../datapipeline-default-role) first.