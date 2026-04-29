---
description: DescribeAccountAssignmentDeletionStatusResponse schema from AWS IAM Identity Center
layout: schema
name: DescribeAccountAssignmentDeletionStatusResponse
properties_list:
- description: ''
  name: AccountAssignmentDeletionStatus
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-describe-account-assignment-deletion-status-response-schema.json
slug: sso-admin-describe-account-assignment-deletion-status-response
source_filename: sso-admin-describe-account-assignment-deletion-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-describe-account-assignment-deletion-status-response-schema.json\",\n  \"title\": \"DescribeAccountAssignmentDeletionStatusResponse\",\n  \"description\": \"DescribeAccountAssignmentDeletionStatusResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountAssignmentDeletionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAssignmentOperationStatus\"\n        },\n        {\n          \"description\": \"The status object for the account assignment deletion operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-describe-account-assignment-deletion-status-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: DescribeAccountAssignmentDeletionStatusResponse
---
