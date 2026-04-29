---
description: AccountList schema
layout: schema
name: AccountList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-account-list-schema.json
slug: inspector-account-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-list-schema.json\",\n  \"title\": \"AccountList\",\n  \"description\": \"AccountList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"accountId\",\n      \"resourceStatus\",\n      \"status\"\n    ],\n    \"properties\": {\n      \"accountId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccountId\"\n          },\n          {\n            \"description\": \"The ID of the Amazon Web Services account.\"\n          }\n        ]\n      },\n      \"resourceStatus\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceStatus\"\n          },\n          {\n            \"description\": \"Details of the status of Amazon Inspector scans by resource type.\"\n  \
  \        }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Status\"\n          },\n          {\n            \"description\": \"The status of Amazon Inspector for the account.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An Amazon Web Services account within your environment that Amazon Inspector has been enabled for.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AccountList
---
