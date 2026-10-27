# Soma Mahapatra

Integration engineer. I design multi-tenant APIs on AWS: one shared API, one role per tenant, and shared stacks parameterized per customer.

## Contact
- Email: somamahapatra1@gmail.com
- GitHub: https://github.com/somamahapatra1-eng

## What I work on

- **CloudFormation.** Nested stacks, mappings, parameters, conditions, and `Fn::Sub`, `Fn::GetAtt`, and `Fn::FindInMap`.
- **IAM.** Resource policies and identity policies, `aws:SourceIp`, `aws:SourceVpce`, role-ID conditions, and least privilege.
- **IAM Roles Anywhere.** Trust anchor, X.509 certificate, profile, and assuming a role from outside AWS. The caller is identified by the assumed-role ARN.
- **API Gateway.** REST API with an IAM (SigV4) authorizer and a Cognito authorizer, plus a resource policy that restricts by source IP.
- **Amazon Cognito.** User pool, ID token (JWT), `cognito:username`, and API Gateway token validation.
- **SigV4 and JWT.** The same Lambda accepts either credential and decides who the caller is.
- **Amazon SQS.** `send_message`, cross-region queues, queue URL, and a queue resource policy.
- **AWS Lambda.** Python and boto3: route the event, read config, and call SQS.
- **AWS AppConfig.** Routing maps choose the queue, so queue URLs are not hardcoded.
- **Amazon S3.** Bucket policy IP allowlist, and presigned URLs.
- **Amazon SNS.** Subscription filter policy by customer, passed into each tenant stack.
- **AWS CodePipeline.** CloudFormation deploy actions, `RunOrder`, and multi-region deploys.
- **VPC endpoints.** Private access to SQS and S3. Resource policies require `aws:SourceVpce`.
- **Multi-tenant design.** One shared API, one role per tenant, shared stacks with per-customer parameters.

## Selected work

Public samples will be linked here. Customer systems stay in their private repositories.
