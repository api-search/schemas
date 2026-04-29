---
description: CreateAccountAssignmentRequest schema from AWS IAM Identity Center
layout: schema
name: CreateAccountAssignmentRequest
properties_list:
- description: ''
  name: InstanceArn
  type: object
- description: ''
  name: TargetId
  type: object
- description: ''
  name: TargetType
  type: object
- description: ''
  name: PermissionSetArn
  type: object
- description: ''
  name: PrincipalType
  type: object
- description: ''
  name: PrincipalId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-create-account-assignment-request-schema.json
slug: sso-admin-create-account-assignment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-create-account-assignment-request-schema.json\",\n  \"title\": \"CreateAccountAssignmentRequest\",\n  \"description\": \"CreateAccountAssignmentRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM Identity Center instance under which the operation will be executed. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"TargetId\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/TargetId\"\n        },\n        {\n          \"description\": \"TargetID is an AWS account identifier, typically a 10-12 digit string (For example, 123456789012).\"\n        }\n      ]\n    },\n    \"TargetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetType\"\n        },\n        {\n          \"description\": \"The entity type for which the assignment will be created.\"\n        }\n      ]\n    },\n    \"PermissionSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetArn\"\n        },\n        {\n          \"description\": \"The ARN of the permission set that the admin wants to grant the principal access to.\"\n        }\n      ]\n    },\n    \"PrincipalType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalType\"\n        },\n        {\n          \"description\": \"The entity type for which the assignment will be created.\"\n       \
  \ }\n      ]\n    },\n    \"PrincipalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalId\"\n        },\n        {\n          \"description\": \"An identifier for an object in IAM Identity Center, such as a user or group. PrincipalIds are GUIDs (For example, f81d4fae-7dec-11d0-a765-00a0c91e6bf6). For more information about PrincipalIds in IAM Identity Center, see the <a href=\\\"/singlesignon/latest/IdentityStoreAPIReference/welcome.html\\\">IAM Identity Center Identity Store API Reference</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceArn\",\n    \"TargetId\",\n    \"TargetType\",\n    \"PermissionSetArn\",\n    \"PrincipalType\",\n    \"PrincipalId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-create-account-assignment-request-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: CreateAccountAssignmentRequest
---
