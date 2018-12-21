# datapipeline default role

Data pipeline default role

To deploy using aws cli:
```sh
aws cloudformation deploy \
  --template-file template.yml \
  --stack-name datapipeline-role \
  --template role-template.yml \
  --capabilities CAPABILITY_NAMED_IAM \
  --profile cloudformation@flowlab-development
```
