---
description: An object with details the status of an Amazon Web Services account within your Amazon Inspector environment.
layout: schema
name: AccountState
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: resourceState
  type: object
- description: ''
  name: state
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-account-state-schema.json
slug: inspector-account-state
source_filename: inspector-account-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-state-schema.json\",\n  \"title\": \"AccountState\",\n  \"description\": \"An object with details the status of an Amazon Web Services account within your Amazon Inspector environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"resourceState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceState\"\n        },\n        {\n          \"description\": \"An object detailing which resources Amazon Inspector is enabled to scan for the account.\"\n        }\n      ]\n    },\n    \"state\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"An object detailing the status of Amazon Inspector for the account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"resourceState\",\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-state-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AccountState
---
