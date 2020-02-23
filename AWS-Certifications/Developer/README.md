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
