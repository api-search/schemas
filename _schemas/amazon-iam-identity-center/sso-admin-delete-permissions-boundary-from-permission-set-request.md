---
description: DeletePermissionsBoundaryFromPermissionSetRequest schema from AWS IAM Identity Center
layout: schema
name: DeletePermissionsBoundaryFromPermissionSetRequest
properties_list:
- description: ''
  name: InstanceArn
  type: object
- description: ''
  name: PermissionSetArn
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-delete-permissions-boundary-from-permission-set-request-schema.json
slug: sso-admin-delete-permissions-boundary-from-permission-set-request
source_filename: sso-admin-delete-permissions-boundary-from-permission-set-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-delete-permissions-boundary-from-permission-set-request-schema.json\",\n  \"title\": \"DeletePermissionsBoundaryFromPermissionSetRequest\",\n  \"description\": \"DeletePermissionsBoundaryFromPermissionSetRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM Identity Center instance under which the operation will be executed. \"\n        }\n      ]\n    },\n    \"PermissionSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetArn\"\n        },\n        {\n          \"description\": \"The ARN of the <code>PermissionSet</code>.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceArn\",\n    \"PermissionSetArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-delete-permissions-boundary-from-permission-set-request-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: DeletePermissionsBoundaryFromPermissionSetRequest
---
