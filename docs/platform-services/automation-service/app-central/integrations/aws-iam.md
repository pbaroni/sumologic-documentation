---
title: AWS IAM
description: ''
tags: []
---

![](/img/platform-services/automation-service/app-central/logos/aws.png)

Version: 1.2  
Updated: Jan 16, 2024

Using the integration with IAM, you can create and manage AWS users and groups, and use permissions to allow and deny their access to AWS resources. 

## Actions

* **Get User** (*Enrichment) -* Retrieves information about the specified IAM user, including the user's creation date, path, unique ID, and ARN
* **List User** (*Enrichment) -* Lists the IAM users that have the specified path prefix
* **List Groups** (*Enrichment) -* Lists the IAM groups that have the specified path prefix
* **List Groups For User** (*Enrichment) -* Lists the IAM groups that the specified IAM user belongs to
* **List Access Key For User** (*Enrichment) -* Returns information about the access key IDs associated with the specified IAM user.
* **List Policies** (*Enrichment) -* Lists all the managed policies that are available in an AWS account
* **List Roles** (*Enrichment) -* Lists the IAM roles that have the specified path prefix
* **List Instance Profiles** (*Enrichment) -* Lists the instance profiles that have the specified path prefix
* **List Instance Profiles For Role** (*Enrichment) -* Lists the instance profiles that have the specified associated IAM role
* **Get Instance Profile** (*Enrichment) -* Returns information about the specified instance profile
* **Get Role** (*Enrichment) -* Retrieves information about the specified role, including the role's path, GUID, ARN, and the role's trust policy that grants permission to assume the role
* **Update User** (*Containment) -* Updates the name and/or the path of the specified IAM user
* **Add User To Group** (*Containment) -* Adds the specified user to the specified group
* **Remove User From Group** (*Containment) -* Removes a specified user from a specified group
* **Delete Access Key** (*Containment) -* Deletes the access key pair associated with the specified IAM user
* **Attach Policy** (*Containment) -* Attaches a policy to the specified target
* **Detach Policy** (*Containment) -* Detaches a policy from a specified target
* **Delete Login Profile** (*Containment) -*Deletes the password for the specified IAM user, which terminates the user's ability to access AWS services through the AWS Management Console
* **Remove Role From Instance** (*Containment) -* Removes the specified IAM role from the specified EC2 instance profile

## External Libraries

* [AWS IAM](https://github.com/boto/boto3/blob/develop/LICENSE)

## Change Log

* October 1, 2019 - First upload
* June 21, 2023 (v1.1) - Updated the integration with Environmental Variables
* January 16, 2024 (v1.2)
	+ Changed the field type of the Access key to password
	+ Updated action: Get User (Table View issue fixed)
