---
description: FreeTrialInfoErrorList schema
layout: schema
name: FreeTrialInfoErrorList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-free-trial-info-error-list-schema.json
slug: inspector-free-trial-info-error-list
source_filename: inspector-free-trial-info-error-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-free-trial-info-error-list-schema.json\",\n  \"title\": \"FreeTrialInfoErrorList\",\n  \"description\": \"FreeTrialInfoErrorList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"accountId\",\n      \"code\",\n      \"message\"\n    ],\n    \"properties\": {\n      \"accountId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/MeteringAccountId\"\n          },\n          {\n            \"description\": \"The account associated with the Amazon Inspector free trial information.\"\n          }\n        ]\n      },\n      \"code\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FreeTrialInfoErrorCode\"\n          },\n          {\n            \"description\": \"The error\
  \ code.\"\n          }\n        ]\n      },\n      \"message\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The error message returned.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about an error received while accessing free trail data for an account.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-free-trial-info-error-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: FreeTrialInfoErrorList
---
