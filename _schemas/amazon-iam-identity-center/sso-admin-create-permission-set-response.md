---
description: CreatePermissionSetResponse schema from AWS IAM Identity Center
layout: schema
name: CreatePermissionSetResponse
properties_list:
- description: ''
  name: PermissionSet
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-create-permission-set-response-schema.json
slug: sso-admin-create-permission-set-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-create-permission-set-response-schema.json\",\n  \"title\": \"CreatePermissionSetResponse\",\n  \"description\": \"CreatePermissionSetResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PermissionSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSet\"\n        },\n        {\n          \"description\": \"Defines the level of access on an AWS account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-create-permission-set-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: CreatePermissionSetResponse
---
