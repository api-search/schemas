---
description: An object that described the state of Amazon Inspector scans for an account.
layout: schema
name: State
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-state-schema.json
slug: inspector-state
source_filename: inspector-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-state-schema.json\",\n  \"title\": \"State\",\n  \"description\": \"An object that described the state of Amazon Inspector scans for an account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorCode\"\n        },\n        {\n          \"description\": \"The error code explaining why the account failed to enable Amazon Inspector.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The error message received when the account failed to enable Amazon Inspector.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The status of Amazon Inspector for the account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errorCode\",\n    \"errorMessage\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-state-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: State
---
