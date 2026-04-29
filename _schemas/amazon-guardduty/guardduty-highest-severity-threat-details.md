---
description: Contains details of the highest severity threat detected during scan and number of infected files.
layout: schema
name: HighestSeverityThreatDetails
properties_list:
- description: ''
  name: Severity
  type: object
- description: ''
  name: ThreatName
  type: object
- description: ''
  name: Count
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-highest-severity-threat-details-schema.json
slug: guardduty-highest-severity-threat-details
source_filename: guardduty-highest-severity-threat-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-highest-severity-threat-details-schema.json\",\n  \"title\": \"HighestSeverityThreatDetails\",\n  \"description\": \"Contains details of the highest severity threat detected during scan and number of infected files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"severity\"\n          },\n          \"description\": \"Severity level of the highest severity threat detected.\"\n        }\n      ]\n    },\n    \"ThreatName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"threatName\"\n          },\n          \"description\"\
  : \"Threat name of the highest severity threat detected as part of the malware scan.\"\n        }\n      ]\n    },\n    \"Count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"count\"\n          },\n          \"description\": \"Total number of infected files with the highest severity threat detected.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-highest-severity-threat-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: HighestSeverityThreatDetails
---
