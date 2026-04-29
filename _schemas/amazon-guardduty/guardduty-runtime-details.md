---
description: Information about the process and any required context values for a specific finding.
layout: schema
name: RuntimeDetails
properties_list:
- description: ''
  name: Process
  type: object
- description: ''
  name: Context
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-runtime-details-schema.json
slug: guardduty-runtime-details
source_filename: guardduty-runtime-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-runtime-details-schema.json\",\n  \"title\": \"RuntimeDetails\",\n  \"description\": \"Information about the process and any required context values for a specific finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Process\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProcessDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"process\"\n          },\n          \"description\": \"Information about the observed process.\"\n        }\n      ]\n    },\n    \"Context\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeContext\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"context\"\n          },\n          \"description\": \"Additional information about the suspicious\
  \ activity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-runtime-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: RuntimeDetails
---
