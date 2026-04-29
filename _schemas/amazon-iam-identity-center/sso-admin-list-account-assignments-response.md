---
description: ListAccountAssignmentsResponse schema from AWS IAM Identity Center
layout: schema
name: ListAccountAssignmentsResponse
properties_list:
- description: ''
  name: AccountAssignments
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-list-account-assignments-response-schema.json
slug: sso-admin-list-account-assignments-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-account-assignments-response-schema.json\",\n  \"title\": \"ListAccountAssignmentsResponse\",\n  \"description\": \"ListAccountAssignmentsResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountAssignments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAssignmentList\"\n        },\n        {\n          \"description\": \"The list of assignments that match the input AWS account and permission set.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"The pagination token for the list API. Initially the value is null. Use the output of previous API calls to\
  \ make subsequent calls.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-account-assignments-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: ListAccountAssignmentsResponse
---
