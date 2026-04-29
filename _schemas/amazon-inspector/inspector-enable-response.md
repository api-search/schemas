---
description: EnableResponse schema
layout: schema
name: EnableResponse
properties_list:
- description: ''
  name: accounts
  type: object
- description: ''
  name: failedAccounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-enable-response-schema.json
slug: inspector-enable-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-enable-response-schema.json\",\n  \"title\": \"EnableResponse\",\n  \"description\": \"EnableResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountList\"\n        },\n        {\n          \"description\": \"Information on the accounts that have had Amazon Inspector scans successfully enabled. Details are provided for each account.\"\n        }\n      ]\n    },\n    \"failedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedAccountList\"\n        },\n        {\n          \"description\": \"Information on any accounts for which Amazon Inspector scans could not be enabled. Details are provided for each account.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"accounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-enable-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: EnableResponse
---
