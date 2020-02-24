https://www.udemy.com/course/aws-certified-developer-associate-dva-c01/learn/lecture/11851550#overview


### decode-authorization-message
see lecture # 65

https://docs.aws.amazon.com/cli/latest/reference/sts/decode-authorization-message.html

$ aws sts decode-authorization-message --encoded-message <msg>
add policy to allow sts decode msg

### AWS EC2 Instance Metadata
see lecture # 66

URL: http://169.254.169.254/latest/meta-data

metadata: info about the EC2 instance
userdata: launch script of the EC2 instance
SSH into ec2 instance
$ curl http://169.254.169.254/latest/meta-data/

### AWS CLI is a wrapper around AWS SDK (boto3/botocore is python API)


### Exponential backoff for rate-limited resources

### AWS profile
$ aws configure --profile <another-aws-account>

Lecture #126 Kinesis KCL
KCL - read record from Streams with distributed app sharing the read workload
Rule: each shard is read by one KCL instance

KCL progress is checkpointed into DynamoDB (need IAM access)

Kinesis data analytics can create streams out of real-time query for down-stream app

Firehose - near real-time (> 60sec) to load data into S3/Redshift/ES/Splunk
with Auto-scaling

Lecture #128 SQS-SNS-Kinesis

Lecture #160 API gateway hands-on
Lecture #161 API gateway stage/deploy

stage variables are passed to Lambda "context" object
mapped to Lambda alias
Canary deployment: choose % of traffic each channel receives (Blue/Green deployment)
why python is not an option in API gateway SDK generator

Lecture #168 API Gateway security
* IAM Permission (only within AWS)
* Lambda authorizer/Custom Authorizer
uses AWS Lambda to validate the token in header: help to use OAuth/SAML/3rd party authentication
* Cognitor User Pools
only for authentication (not authorization)





