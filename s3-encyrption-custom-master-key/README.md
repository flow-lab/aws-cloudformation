# s3-encryption-custom-master-key

Turn on KMS encryption on s3 by default with custom KMS Customer Master Key.

To deploy using aws cli:
```sh
aws cloudformation deploy \
  --template-file template.yml \
  --stack-name s3-encryption-template \
  --template s3-template.yml \
  --profile cloudformation@flowlab-development
```
