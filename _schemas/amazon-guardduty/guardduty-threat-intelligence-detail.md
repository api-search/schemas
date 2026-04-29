---
description: An instance of a threat intelligence detail that constitutes evidence for the finding.
layout: schema
name: ThreatIntelligenceDetail
properties_list:
- description: ''
  name: ThreatListName
  type: object
- description: ''
  name: ThreatNames
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-threat-intelligence-detail-schema.json
slug: guardduty-threat-intelligence-detail
source_filename: guardduty-threat-intelligence-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-threat-intelligence-detail-schema.json\",\n  \"title\": \"ThreatIntelligenceDetail\",\n  \"description\": \"An instance of a threat intelligence detail that constitutes evidence for the finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ThreatListName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"threatListName\"\n          },\n          \"description\": \"The name of the threat intelligence list that triggered the finding.\"\n        }\n      ]\n    },\n    \"ThreatNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThreatNames\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"threatNames\"\n          },\n    \
  \      \"description\": \"A list of names of the threats in the threat intelligence list that triggered the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-threat-intelligence-detail-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ThreatIntelligenceDetail
---
