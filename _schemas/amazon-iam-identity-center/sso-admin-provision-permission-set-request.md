---
description: ProvisionPermissionSetRequest schema from AWS IAM Identity Center
layout: schema
name: ProvisionPermissionSetRequest
properties_list:
- description: ''
  name: InstanceArn
  type: object
- description: ''
  name: PermissionSetArn
  type: object
- description: ''
  name: TargetId
  type: object
- description: ''
  name: TargetType
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-provision-permission-set-request-schema.json
slug: sso-admin-provision-permission-set-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-provision-permission-set-request-schema.json\",\n  \"title\": \"ProvisionPermissionSetRequest\",\n  \"description\": \"ProvisionPermissionSetRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM Identity Center instance under which the operation will be executed. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"PermissionSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/PermissionSetArn\"\n        },\n        {\n          \"description\": \"The ARN of the permission set.\"\n        }\n      ]\n    },\n    \"TargetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetId\"\n        },\n        {\n          \"description\": \"TargetID is an AWS account identifier, typically a 10-12 digit string (For example, 123456789012).\"\n        }\n      ]\n    },\n    \"TargetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisionTargetType\"\n        },\n        {\n          \"description\": \"The entity type for which the assignment will be created.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceArn\",\n    \"PermissionSetArn\",\n    \"TargetType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-provision-permission-set-request-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: ProvisionPermissionSetRequest
---
