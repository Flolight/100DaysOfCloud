
![security](./img1.jpg)

# [AWS] Sagemaker #1 - Security

## Introduction

I'm really close to the AWS Machine Learning exam and Security is a pretty important topic for machine learning, considering the sensitive data you might deal with and the costly infrastructure you need to manage.

## Cloud Research

Main resource for this topic is (as often) the [Sagemaker Developper guide](https://docs.aws.amazon.com/sagemaker/latest/dg/security.html).

- You should as always encrypt your data at rest:

That means using KMS key to encrypt any storage associated to your notebook instances (or any other ML tool: jobs, endpoints...) and S3 buckets.

- Encrypt data in transit:

For inter-container encryption (private VPC) between training instances, be aware it can increase training time especially for deep learning algorithms.

- IAM: noting really new here, just some reminders

Least privilege priciple, roles, policies, access from another account / ouside the organization...

- Enable login with Cloutrail
- Another useful resource: [sagemaker workshops](https://sagemaker-workshop.com/) by [@moviolone](https://twitter.com/moviolone)

## Social Proof

[The tweet](https://twitter.com/FlolightC/status/1312385403278757895)
