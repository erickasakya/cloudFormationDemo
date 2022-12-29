## CloudFormation Test

After configuring the aws cli on your local pc run the command below to create the cf vpc
``` aws cloudformation create-stack --stack-name firstcfvpc --region us-east-1 --template-body file://vpc.yaml --profile udacity_user ```

To update the stack use the command below
``` aws cloudformation update-stack --stack-name firstcfvpc --region us-east-1 --template-body file://vpc.yaml --profile udacity_user ```

To view the status of the stack you can use the below command or use AWS management console
```aws cloudformation describe-stacks --stack-name firstcfvpc --profile udacity_user```
{
    "Stacks": [
        {
            "StackId": "arn:aws:cloudformation:us-east-1:552774009404:stack/firstcfvpc/71394840-7c2f-11ed-8705-0adbb06ea993",
            "StackName": "firstcfvpc",
            "Description": "Eric Kasakya / Software Engineer - This is CloudFormations deploys VPC",
            "CreationTime": "2022-12-15T04:17:52.446000+00:00",
            "RollbackConfiguration": {},
            "StackStatus": "CREATE_COMPLETE",
            "DisableRollback": false,
            "NotificationARNs": [],
            "Tags": [],
            "EnableTerminationProtection": false,
            "DriftInformation": {
                "StackDriftStatus": "NOT_CHECKED"
            }
        }
    ]
}
