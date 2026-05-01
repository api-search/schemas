---
description: CreateAccountAssignmentResponse schema from AWS IAM Identity Center
layout: schema
name: CreateAccountAssignmentResponse
properties_list:
- description: ''
  name: AccountAssignmentCreationStatus
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-create-account-assignment-response-schema.json
slug: sso-admin-create-account-assignment-response
source_filename: sso-admin-create-account-assignment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-create-account-assignment-response-schema.json\",\n  \"title\": \"CreateAccountAssignmentResponse\",\n  \"description\": \"CreateAccountAssignmentResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountAssignmentCreationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAssignmentOperationStatus\"\n        },\n        {\n          \"description\": \"The status object for the account assignment creation operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-create-account-assignment-response-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: CreateAccountAssignmentResponse
---
