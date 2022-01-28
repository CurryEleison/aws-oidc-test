# AWS / GitHub OpenID Connect Test

Demo of OpenID Connect between AWS and GitHub Actions:
- No Access/Secret key stored in GitHub Actions Secrets -- permissions handled by OIDC
- Builds a multiarch python container with boto3 and pushes it to ECR

Steps to reproduce available at https://benoitboure.com/securely-access-your-aws-resources-from-github-actions

Useful CloudFormation template to set up the requisite role (and optionally the identity provider) 
at AWS: https://github.com/aws-actions/configure-aws-credentials#sample-iam-role-cloudformation-template . 
(Note the clever trick where you can supply an OIDC ARN or have a new one created by the template!)

