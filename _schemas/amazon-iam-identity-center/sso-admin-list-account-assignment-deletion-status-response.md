---
description: ListAccountAssignmentDeletionStatusResponse schema from AWS IAM Identity Center
layout: schema
name: ListAccountAssignmentDeletionStatusResponse
properties_list:
- description: ''
  name: AccountAssignmentsDeletionStatus
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-list-account-assignment-deletion-status-response-schema.json
slug: sso-admin-list-account-assignment-deletion-status-response
source_filename: sso-admin-list-account-assignment-deletion-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-account-assignment-deletion-status-response-schema.json\",\n  \"title\": \"ListAccountAssignmentDeletionStatusResponse\",\n  \"description\": \"ListAccountAssignmentDeletionStatusResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountAssignmentsDeletionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAssignmentOperationStatusList\"\n        },\n        {\n          \"description\": \"The status object for the account assignment deletion operation.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"The pagination token for the list API. Initially\
  \ the value is null. Use the output of previous API calls to make subsequent calls.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-account-assignment-deletion-status-response-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: ListAccountAssignmentDeletionStatusResponse
---
