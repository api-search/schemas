---
description: DelegatedAdminAccountList schema
layout: schema
name: DelegatedAdminAccountList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-delegated-admin-account-list-schema.json
slug: inspector-delegated-admin-account-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-delegated-admin-account-list-schema.json\",\n  \"title\": \"DelegatedAdminAccountList\",\n  \"description\": \"DelegatedAdminAccountList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"accountId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccountId\"\n          },\n          {\n            \"description\": \"The Amazon Web Services account ID of the Amazon Inspector delegated administrator for your organization.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DelegatedAdminStatus\"\n          },\n          {\n            \"description\": \"The status of the Amazon Inspector delegated administrator.\"\n\
  \          }\n        ]\n      }\n    },\n    \"description\": \"Details of the Amazon Inspector delegated administrator for your organization.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-delegated-admin-account-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: DelegatedAdminAccountList
---
