# Basic EC2 Workshop for Awesome People

## Preparation

So [follow these instructions to install AWS-CLI first](https://docs.aws.amazon.com/cli/latest/userguide/cli-install-macos.html)

# Basic commands

Create stuff:

```
aws cloudformation create-stack --region ap-southeast-2 --stack-name BANANASTACK --template-body file://banana.yaml \
--parameters banana-params.json 
```

Delete stuff:

```
aws cloudformation delete-stack --region ap-southeast-2 --stack-name BANANASTACK
```

What's in my stack?

```
aws cloudformation describe-stacks --region ap-southeast-2 --stack-name BANANASTACK
```

