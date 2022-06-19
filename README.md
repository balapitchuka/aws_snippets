# AWS

## References
- [AWS Sample Code Snippets](https://github.com/aws-samples)


## Other Prerequisites
- [JMESPath language](https://jmespath.org/tutorial.html)

## Tools
- [Subnet calculator](https://www.davidc.net/sites/default/subnets/subnets.html)

## AWS CLI Command Reference
Find availability zones that exist for your account in any given region
```
aws --profile=cloudcasts ec2 describe-availability-zones --region us-east-2
```

```
aws --profile=cloudcasts ec2 describe-availability-zones \
    --region us-east-2 \
    --query 'AvailabilityZones[].ZoneName'
 
# Output:
[
    "us-east-2a",
    "us-east-2b",
    "us-east-2c"
]
```





