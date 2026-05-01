---
description: GetPermissionsBoundaryForPermissionSetResponse schema from AWS IAM Identity Center
layout: schema
name: GetPermissionsBoundaryForPermissionSetResponse
properties_list:
- description: ''
  name: PermissionsBoundary
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-get-permissions-boundary-for-permission-set-response-schema.json
slug: sso-admin-get-permissions-boundary-for-permission-set-response
source_filename: sso-admin-get-permissions-boundary-for-permission-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-get-permissions-boundary-for-permission-set-response-schema.json\",\n  \"title\": \"GetPermissionsBoundaryForPermissionSetResponse\",\n  \"description\": \"GetPermissionsBoundaryForPermissionSetResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PermissionsBoundary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionsBoundary\"\n        },\n        {\n          \"description\": \"The permissions boundary attached to the specified permission set.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-get-permissions-boundary-for-permission-set-response-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: GetPermissionsBoundaryForPermissionSetResponse
---
