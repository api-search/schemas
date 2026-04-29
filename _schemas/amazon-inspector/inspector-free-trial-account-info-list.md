---
description: FreeTrialAccountInfoList schema
layout: schema
name: FreeTrialAccountInfoList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-free-trial-account-info-list-schema.json
slug: inspector-free-trial-account-info-list
source_filename: inspector-free-trial-account-info-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-free-trial-account-info-list-schema.json\",\n  \"title\": \"FreeTrialAccountInfoList\",\n  \"description\": \"FreeTrialAccountInfoList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"accountId\",\n      \"freeTrialInfo\"\n    ],\n    \"properties\": {\n      \"accountId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/MeteringAccountId\"\n          },\n          {\n            \"description\": \"The account associated with the Amazon Inspector free trial information.\"\n          }\n        ]\n      },\n      \"freeTrialInfo\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FreeTrialInfoList\"\n          },\n          {\n            \"description\": \"Contains information\
  \ about the Amazon Inspector free trial for an account.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about the Amazon Inspector free trial for an account.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-free-trial-account-info-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: FreeTrialAccountInfoList
---
