# aws-iam-least-privilege-remediation
This project demonstrates the transition from a high-risk AdministratorAccess model to a hardened Least-Privilege security posture. I identified an over-privileged developer account, audited its actual usage, and authored a custom JSON policy to restrict permissions to only necessary actions, effectively reducing the account's attack surface.
```json
{
"Version": "2012-10-17",
"Statement": [
{
"Effect": "Allow",
"Action": [
"s3:GetObject",
"s3:PutObject",
"s3:ListBucket"
],
"Resource": "*"
}
]
}
```
