---
description: Contains details about identified threats organized by threat name.
layout: schema
name: ThreatDetectedByName
properties_list:
- description: ''
  name: ItemCount
  type: object
- description: ''
  name: UniqueThreatNameCount
  type: object
- description: ''
  name: Shortened
  type: object
- description: ''
  name: ThreatNames
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-threat-detected-by-name-schema.json
slug: guardduty-threat-detected-by-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-threat-detected-by-name-schema.json\",\n  \"title\": \"ThreatDetectedByName\",\n  \"description\": \"Contains details about identified threats organized by threat name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ItemCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"itemCount\"\n          },\n          \"description\": \"Total number of infected files identified.\"\n        }\n      ]\n    },\n    \"UniqueThreatNameCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"uniqueThreatNameCount\"\n          },\n          \"description\": \"Total number of unique\
  \ threats by name identified, as part of the malware scan.\"\n        }\n      ]\n    },\n    \"Shortened\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shortened\"\n          },\n          \"description\": \"Flag to determine if the finding contains every single infected file-path and/or every threat.\"\n        }\n      ]\n    },\n    \"ThreatNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanThreatNames\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"threatNames\"\n          },\n          \"description\": \"List of identified threats with details, organized by threat name.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-threat-detected-by-name-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ThreatDetectedByName
---
