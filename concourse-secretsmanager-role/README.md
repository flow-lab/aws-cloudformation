# Concourse AWS SecretsManager role

Concourse AWS SecretsManager role

To deploy using aws cli:
```sh
aws cloudformation deploy \
  --template-file template.yml \
  --stack-name ConcourseSecretsManagerRole \
  --template role-template.yml \
  --capabilities CAPABILITY_NAMED_IAM \
  --profile cloud-formation@flowlab-development
```
