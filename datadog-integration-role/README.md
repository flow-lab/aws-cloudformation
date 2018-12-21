# datadog-aws

DatadogAWSIntegrationRole - ref [datadog AWS doc](https://docs.datadoghq.com/integrations/amazon_web_services/#installation)

To deploy using aws cli:
```sh
aws cloudformation create-stack --stack-name datadog-integration-role \
  --template-body file://integration-role/integration-role.yml \
  --parameters ParameterKey=ExternalID,ParameterValue="AWS External ID" \
  --capabilities CAPABILITY_NAMED_IAM \
  --profile cloudformation@flowlab-development
```