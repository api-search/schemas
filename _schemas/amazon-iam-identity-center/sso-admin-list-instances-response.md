---
description: ListInstancesResponse schema from AWS IAM Identity Center
layout: schema
name: ListInstancesResponse
properties_list:
- description: ''
  name: Instances
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-list-instances-response-schema.json
slug: sso-admin-list-instances-response
source_filename: sso-admin-list-instances-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-instances-response-schema.json\",\n  \"title\": \"ListInstancesResponse\",\n  \"description\": \"ListInstancesResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Instances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceList\"\n        },\n        {\n          \"description\": \"Lists the IAM Identity Center instances that the caller has access to.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"The pagination token for the list API. Initially the value is null. Use the output of previous API calls to make subsequent calls.\"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-instances-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: ListInstancesResponse
---
