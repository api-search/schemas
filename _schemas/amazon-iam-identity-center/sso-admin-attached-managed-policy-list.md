---
description: AttachedManagedPolicyList schema from AWS IAM Identity Center
layout: schema
name: AttachedManagedPolicyList
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-attached-managed-policy-list-schema.json
slug: sso-admin-attached-managed-policy-list
source_filename: sso-admin-attached-managed-policy-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-attached-managed-policy-list-schema.json\",\n  \"title\": \"AttachedManagedPolicyList\",\n  \"description\": \"AttachedManagedPolicyList schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The name of the AWS managed policy.\"\n          }\n        ]\n      },\n      \"Arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ManagedPolicyArn\"\n          },\n          {\n            \"description\": \"The ARN of the AWS managed policy. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\
  \">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A structure that stores the details of the AWS managed policy.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-attached-managed-policy-list-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: AttachedManagedPolicyList
---
