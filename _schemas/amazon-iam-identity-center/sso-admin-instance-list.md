---
description: InstanceList schema from AWS IAM Identity Center
layout: schema
name: InstanceList
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-instance-list-schema.json
slug: sso-admin-instance-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-instance-list-schema.json\",\n  \"title\": \"InstanceList\",\n  \"description\": \"InstanceList schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"InstanceArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/InstanceArn\"\n          },\n          {\n            \"description\": \"The ARN of the IAM Identity Center instance under which the operation will be executed. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\n          }\n        ]\n      },\n      \"IdentityStoreId\": {\n        \"allOf\": [\n          {\n\
  \            \"$ref\": \"#/components/schemas/Id\"\n          },\n          {\n            \"description\": \"The identifier of the identity store that is connected to the IAM Identity Center instance.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Provides information about the IAM Identity Center instance.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-instance-list-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: InstanceList
---
