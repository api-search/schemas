---
description: Total number of scanned files.
layout: schema
name: ScannedItemCount
properties_list:
- description: ''
  name: TotalGb
  type: object
- description: ''
  name: Files
  type: object
- description: ''
  name: Volumes
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scanned-item-count-schema.json
slug: guardduty-scanned-item-count
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scanned-item-count-schema.json\",\n  \"title\": \"ScannedItemCount\",\n  \"description\": \"Total number of scanned files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TotalGb\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"totalGb\"\n          },\n          \"description\": \"Total GB of files scanned for malware.\"\n        }\n      ]\n    },\n    \"Files\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"files\"\n          },\n          \"description\": \"Number of files scanned.\"\n        }\n      ]\n    },\n    \"Volumes\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumes\"\n          },\n          \"description\": \"Total number of scanned volumes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scanned-item-count-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScannedItemCount
---
