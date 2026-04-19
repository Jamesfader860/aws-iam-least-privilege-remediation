<img width="1333" height="520" alt="01-iam-user-setup" src="https://github.com/user-attachments/assets/8f8e6ab7-4c1e-4088-b51a-af9a76b6dd0b" />
<img width="1318" height="502" alt="02-overprivileged-admin" src="https://github.com/user-attachments/assets/4ef2b121-ddd2-49df-8f85-b4cfe071d2b1" />
<img width="1307" height="428" alt="03-risk-verification-test" src="https://github.com/user-attachments/assets/f2e4a1e7-7df1-4991-92ec-3a88b3ae87a3" />
<img width="1334" height="534" alt="04-access-analyzer-audit" src="https://github.com/user-attachments/assets/ba68302c-87d4-4418-a498-cce80a4fa77d" />
<img width="1306" height="455" alt="05-iam-wildcard-policy-draft" src="https://github.com/user-attachments/assets/00bc01dc-e61c-4d98-8873-501dfb710457" />
<img width="1300" height="523" alt="06-least-privilege-json" src="https://github.com/user-attachments/assets/6d8ead4f-d5ce-446f-9537-07c1305e23d9" />
<img width="1321" height="412" alt="07-policy-selection-step" src="https://github.com/user-attachments/assets/971a5eb5-bc82-4506-9f7d-494bc205496f" />
<img width="1310" height="468" alt="08-custom-policy-provisioned" src="https://github.com/user-attachments/assets/54ae4c73-4aca-443b-a210-2b53b1402002" />
<img width="1298" height="467" alt="09-final-security-validation" src="https://github.com/user-attachments/assets/93348f82-43ed-4786-b082-2392e081e20d" />



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
