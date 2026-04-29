---
description: ListAccountAssignmentCreationStatusResponse schema from AWS IAM Identity Center
layout: schema
name: ListAccountAssignmentCreationStatusResponse
properties_list:
- description: ''
  name: AccountAssignmentsCreationStatus
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-list-account-assignment-creation-status-response-schema.json
slug: sso-admin-list-account-assignment-creation-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-account-assignment-creation-status-response-schema.json\",\n  \"title\": \"ListAccountAssignmentCreationStatusResponse\",\n  \"description\": \"ListAccountAssignmentCreationStatusResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountAssignmentsCreationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAssignmentOperationStatusList\"\n        },\n        {\n          \"description\": \"The status object for the account assignment creation operation.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"The pagination token for the list API. Initially\
  \ the value is null. Use the output of previous API calls to make subsequent calls.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-account-assignment-creation-status-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: ListAccountAssignmentCreationStatusResponse
---
