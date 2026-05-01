---
description: AccountStateList schema
layout: schema
name: AccountStateList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-account-state-list-schema.json
slug: inspector-account-state-list
source_filename: inspector-account-state-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-state-list-schema.json\",\n  \"title\": \"AccountStateList\",\n  \"description\": \"AccountStateList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"accountId\",\n      \"resourceState\",\n      \"state\"\n    ],\n    \"properties\": {\n      \"accountId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccountId\"\n          },\n          {\n            \"description\": \"The Amazon Web Services account ID.\"\n          }\n        ]\n      },\n      \"resourceState\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceState\"\n          },\n          {\n            \"description\": \"An object detailing which resources Amazon Inspector is enabled to\
  \ scan for the account.\"\n          }\n        ]\n      },\n      \"state\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/State\"\n          },\n          {\n            \"description\": \"An object detailing the status of Amazon Inspector for the account.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object with details the status of an Amazon Web Services account within your Amazon Inspector environment.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-state-list-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AccountStateList
---
