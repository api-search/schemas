---
description: BatchGetFreeTrialInfoResponse schema
layout: schema
name: BatchGetFreeTrialInfoResponse
properties_list:
- description: ''
  name: accounts
  type: object
- description: ''
  name: failedAccounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-free-trial-info-response-schema.json
slug: inspector-batch-get-free-trial-info-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-free-trial-info-response-schema.json\",\n  \"title\": \"BatchGetFreeTrialInfoResponse\",\n  \"description\": \"BatchGetFreeTrialInfoResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FreeTrialAccountInfoList\"\n        },\n        {\n          \"description\": \"An array of objects that provide Amazon Inspector free trial details for each of the requested accounts. \"\n        }\n      ]\n    },\n    \"failedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FreeTrialInfoErrorList\"\n        },\n        {\n          \"description\": \"An array of objects detailing any accounts that free trial data could not be returned for.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"accounts\",\n    \"failedAccounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-free-trial-info-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetFreeTrialInfoResponse
---
