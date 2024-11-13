---
title: "Identity Access Management (iam)"
datePublished: Wed Nov 13 2024 21:26:14 GMT+0000 (Coordinated Universal Time)
cuid: cm3ge58az000209jo6qzpbbi3
slug: iam
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1731532875756/c9cebafd-b4d9-4524-87c8-4c77581997b6.png
tags: data, aws, data-science, iam, aws-iam

---

IAM is one of the core concepts in AWS. It’s essential to understand when working with the cloud because it controls access to resources like S3 buckets, EC2 instances, DynamoDB, and many other AWS services.

IAM is responsible for managing both authentication and authorization. This means it controls who can access AWS resources (authentication) and what actions they can perform (authorization) through a permissions-based system.

For example, imagine a computer lab where the instructor represents IAM. The instructor has full control over the lab and can assign specific tasks to students. Each student has access only to the resources and tasks assigned to them by the instructor, preventing them from accessing or modifying other resources without permission.

Additionally, sometimes the instructor assigns group projects where multiple students work together. The instructor has the authority to manage group memberships, like adding or removing students from the project based on their performance.

Similarly, in AWS, It is possible to share the root access with other people who work in the company , and they can delete the resources. So prevent the resources IAM ( authentication and authorization ) 

 IAM manages access to over 200 services such as EC2, DB, KS8, etc. The account owner (root user) has the highest level of access, but they can create IAM users and roles with specific permissions, limiting access to resources based on defined policies.

**Policies** are sets of rules that specify what actions users, groups, or roles can perform on AWS resources. Whenever we create a user we have assigned the policy otherwise the goal is not clear what can a user do. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXedD9HTfA81BInEyjGbw4kq_CrZW3yiiJk0HgqJr7sJEXvlqEfXGazgN7YqJ4IqclLR9RuSXDL1BUZNR_SEgPAJWCKYoNlvNkoMNH-5iTEQgm391Ict4g6BvNX_6mi-ILAHp2QDrg?key=y4V9W8DxIR9d8BHapFLVgm0S align="left")

**Groups:** It is vital that a company have multiple user categories, such as Developer, QA, Database, etc. 

**Roles:** a **role** as a temporary "identity". It’s like the user but not completely doing what a user can. There are some types of rules  *Service-to-Service Access (EC2 accessing S3), Cross-Account Access, Temporary Access for Users* 

When a user attempts to perform Actions on resources, like creating an EC2 instance, authorization to perform an Action depends on a policy. 

**How do you create a User?**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1731532980494/411c6715-3145-4ce7-ae0d-00c359a4e658.png align="center")

`Reference`

aws - [https://us-east-1.console.aws.amazon.com/iam/home?region=ap-southeast-2#/users](https://us-east-1.console.aws.amazon.com/iam/home?region=ap-southeast-2#/users)