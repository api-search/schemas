---
description: An entity that contains IAM policies.
layout: schema
name: PermissionSet
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: PermissionSetArn
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: CreatedDate
  type: object
- description: ''
  name: SessionDuration
  type: object
- description: ''
  name: RelayState
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-permission-set-schema.json
slug: sso-admin-permission-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-permission-set-schema.json\",\n  \"title\": \"PermissionSet\",\n  \"description\": \"An entity that contains IAM policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetName\"\n        },\n        {\n          \"description\": \"The name of the permission set.\"\n        }\n      ]\n    },\n    \"PermissionSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetArn\"\n        },\n        {\n          \"description\": \"The ARN of the permission set. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\
  \n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetDescription\"\n        },\n        {\n          \"description\": \"The description of the <a>PermissionSet</a>.\"\n        }\n      ]\n    },\n    \"CreatedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date that the permission set was created.\"\n        }\n      ]\n    },\n    \"SessionDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"The length of time that the application user sessions are valid for in the ISO-8601 standard.\"\n        }\n      ]\n    },\n    \"RelayState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelayState\"\n        },\n        {\n          \"description\": \"Used to redirect users within\
  \ the application during the federation authentication process.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-permission-set-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: PermissionSet
---
