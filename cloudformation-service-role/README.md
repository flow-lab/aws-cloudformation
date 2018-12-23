# cloudformation service role

CloudFormation service role

To deploy using aws cli:
```sh
aws cloudformation deploy \
  --template-file template.yml \
  --stack-name cloudformation-service-role \
  --template role-template.yml \
  --capabilities CAPABILITY_NAMED_IAM \
  --profile cloudformation@flowlab-development
```
