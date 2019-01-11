# flow-datapipeline

Data pipeline that runs [flow](https://github.com/flow-lab/flow) cli. For example to run purging of DynamoDB table.

To deploy using aws cli:
```sh
aws cloudformation deploy \
    --template-file template.yml \
    --stack-name flow-tooling \
    --parameter-overrides FlowVersion="v0.1.51" FlowCommand="AWS_REGION=eu-west-1 flow dynamodb purge --table-name test" \
    --template datapipeline-template.yml \
    --profile cloudformation@flowlab-development
```

Other low examples:
```sh
flow dynamodb search --table-name Test --filter-expression "id = :id" --expression-attribute-values '{":id":{"S":"1"}}'
flow dynamodb search --table-name Test --filter-expression "attribute_exists(id)" --projection-expression "animalId"
```

If you need a scheduler: [https://docs.aws.amazon.com/datapipeline/latest/DeveloperGuide/dp-object-schedule.html](https://docs.aws.amazon.com/datapipeline/latest/DeveloperGuide/dp-object-schedule.html)
