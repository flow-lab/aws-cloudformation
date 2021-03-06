# aws-cloudformation

CloudFormation templates:

1. [dynamodb-to-dynamodb-datapipeline](./dynamodb-to-dynamodb-datapipeline) - Copy items between DynamoDB tables using S3 
bucket as a temporal storage

2. [datapipeline-default-role](./datapipeline-default-role) - Data Pipeline default role

3. [cloudformation-service-role](./cloudformation-service-role) - [cloudformation-service-role](https://docs.datadoghq.com/integrations/amazon_web_services) integration role

4. [datadog-integratkon-role](./datadog-integration-role) - [Datadog AWS](https://docs.datadoghq.com/integrations/amazon_web_services) integration role

5. [concourse-secretsmanager-role](./concourse-secretsmanager-role) - [Concourse - Credential Management](https://concourse-ci.org/creds.html#configuration)

6. [flow-datapipeline](./flow-datapipeline) - Runs [flow](https://github.com/flow-lab/flow) cli

7. [s3-encyrption-custom-master-key](./s3-encyrption-custom-master-key) - Turn on KMS encryption on s3 by default with custom KMS Customer Master Key

8. [redis](./redis) - ElasticCache redis cluster