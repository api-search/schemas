---
description: A structure that stores the details of the AWS managed policy.
layout: schema
name: AttachedManagedPolicy
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Arn
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-attached-managed-policy-schema.json
slug: sso-admin-attached-managed-policy
source_filename: sso-admin-attached-managed-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-attached-managed-policy-schema.json\",\n  \"title\": \"AttachedManagedPolicy\",\n  \"description\": \"A structure that stores the details of the AWS managed policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the AWS managed policy.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManagedPolicyArn\"\n        },\n        {\n          \"description\": \"The ARN of the AWS managed policy. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in\
  \ the <i>AWS General Reference</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-attached-managed-policy-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: AttachedManagedPolicy
---
