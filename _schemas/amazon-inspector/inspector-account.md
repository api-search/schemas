---
description: An Amazon Web Services account within your environment that Amazon Inspector has been enabled for.
layout: schema
name: Account
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: resourceStatus
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-account-schema.json
slug: inspector-account
source_filename: inspector-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"An Amazon Web Services account within your environment that Amazon Inspector has been enabled for.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"resourceStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStatus\"\n        },\n        {\n          \"description\": \"Details of the status of Amazon Inspector scans by resource type.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\
  \n        },\n        {\n          \"description\": \"The status of Amazon Inspector for the account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"resourceStatus\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Account
---
