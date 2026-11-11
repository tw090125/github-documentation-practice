
# GitHub Documentation Practice

## Project Overview
This repository is dedicated to practicing
technical documentation using GitHub Markdown.

## Objectives
- Learn how to write professional README files
- Document cloud infrastructure projects
- Practice GitHub version control
- Improve technical communication skills

## Technologies
- GitHub
- Markdown
- AWS
- Git

## Lessons Learned
Documentation helps engineers understand,
maintain, and troubleshoot technical systems.

---

# AWS IAM Lab: User and Group Management

## Project Overview

This lab demonstrates how to create and manage
AWS IAM users, groups, and permissions using
the AWS Management Console.

The objective is to practice identity and
access management while applying the
principle of least privilege.

## Business Problem

Organizations need to control who can access
cloud resources and what actions users can perform.

Managing permissions through IAM groups
simplifies access management and helps
maintain consistent security policies.

## Task 1: Create an IAM User

### Implementation

1. Opened the AWS IAM Console.
2. Navigated to IAM Users.
3. Created a user named `devops-lab-user`.
4. Enabled AWS Management Console access.
5. Assigned permissions through an IAM group.
6. Verified the user's access configuration.

### Configuration

| Setting | Value |
|---------|-------|
| Username | devops-lab-user |
| Access Type | AWS Management Console |
| Group | Developers |
| Policy | AmazonS3ReadOnlyAccess |
| Access Keys | None |

### Validation

Confirmed the user was created successfully,
console access was enabled, and permissions
were inherited from the Developers group.

## Task 2: Create an IAM Group

### Implementation

1. Created an IAM group named `Developers`.
2. Attached the AWS-managed policy
   `AmazonS3ReadOnlyAccess`.
3. Added `devops-lab-user` to the group.
4. Verified the user's inherited permissions.

### Security Considerations

Permissions were assigned through group
membership rather than attaching broad
permissions directly to the user.

This approach simplifies permission management
and supports least-privilege access.

## Lessons Learned

- IAM users represent identities in AWS.
- IAM groups simplify permission management.
- IAM policies define allowed actions.
- Users inherit permissions from their groups.
- Least privilege reduces unnecessary access.
- MFA adds protection to console sign-in.

## Next Steps

- Verify group membership and capture evidence.
- Enable MFA for the IAM user.
- Practice creating custom IAM policies.
- Create an IAM role for an AWS service.
