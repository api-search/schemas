---
description: GetInlinePolicyForPermissionSetResponse schema from AWS IAM Identity Center
layout: schema
name: GetInlinePolicyForPermissionSetResponse
properties_list:
- description: ''
  name: InlinePolicy
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-get-inline-policy-for-permission-set-response-schema.json
slug: sso-admin-get-inline-policy-for-permission-set-response
source_filename: sso-admin-get-inline-policy-for-permission-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-get-inline-policy-for-permission-set-response-schema.json\",\n  \"title\": \"GetInlinePolicyForPermissionSetResponse\",\n  \"description\": \"GetInlinePolicyForPermissionSetResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InlinePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetPolicyDocument\"\n        },\n        {\n          \"description\": \"The inline policy that is attached to the permission set.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-get-inline-policy-for-permission-set-response-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: GetInlinePolicyForPermissionSetResponse
---
