---
description: ListPermissionSetsProvisionedToAccountResponse schema from AWS IAM Identity Center
layout: schema
name: ListPermissionSetsProvisionedToAccountResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: PermissionSets
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-list-permission-sets-provisioned-to-account-response-schema.json
slug: sso-admin-list-permission-sets-provisioned-to-account-response
source_filename: sso-admin-list-permission-sets-provisioned-to-account-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-permission-sets-provisioned-to-account-response-schema.json\",\n  \"title\": \"ListPermissionSetsProvisionedToAccountResponse\",\n  \"description\": \"ListPermissionSetsProvisionedToAccountResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"The pagination token for the list API. Initially the value is null. Use the output of previous API calls to make subsequent calls.\"\n        }\n      ]\n    },\n    \"PermissionSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetList\"\n        },\n        {\n          \"description\": \"Defines the\
  \ level of access that an AWS account has.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-permission-sets-provisioned-to-account-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: ListPermissionSetsProvisionedToAccountResponse
---
