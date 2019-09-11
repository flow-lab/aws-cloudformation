# redis

CloudFormation template to create Redis server.

To deploy using aws cli:
```sh
aws cloudformation deploy \
    --template-file template.yml \
    --stack-name redis \
    --template redis-template.yml \
    --profile cloudformation@flowlab-development
```
