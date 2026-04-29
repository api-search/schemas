---
description: UpdatePermissionSetRequest schema from AWS IAM Identity Center
layout: schema
name: UpdatePermissionSetRequest
properties_list:
- description: ''
  name: InstanceArn
  type: object
- description: ''
  name: PermissionSetArn
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: SessionDuration
  type: object
- description: ''
  name: RelayState
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-update-permission-set-request-schema.json
slug: sso-admin-update-permission-set-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-update-permission-set-request-schema.json\",\n  \"title\": \"UpdatePermissionSetRequest\",\n  \"description\": \"UpdatePermissionSetRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM Identity Center instance under which the operation will be executed. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"PermissionSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetArn\"\
  \n        },\n        {\n          \"description\": \"The ARN of the permission set.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetDescription\"\n        },\n        {\n          \"description\": \"The description of the <a>PermissionSet</a>.\"\n        }\n      ]\n    },\n    \"SessionDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"The length of time that the application user sessions are valid for in the ISO-8601 standard.\"\n        }\n      ]\n    },\n    \"RelayState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelayState\"\n        },\n        {\n          \"description\": \"Used to redirect users within the application during the federation authentication process.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceArn\",\n    \"\
  PermissionSetArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-update-permission-set-request-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: UpdatePermissionSetRequest
---
