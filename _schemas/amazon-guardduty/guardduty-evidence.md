---
description: Contains information about the reason that the finding was generated.
layout: schema
name: Evidence
properties_list:
- description: ''
  name: ThreatIntelligenceDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-evidence-schema.json
slug: guardduty-evidence
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-evidence-schema.json\",\n  \"title\": \"Evidence\",\n  \"description\": \"Contains information about the reason that the finding was generated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ThreatIntelligenceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThreatIntelligenceDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"threatIntelligenceDetails\"\n          },\n          \"description\": \"A list of threat intelligence details related to the evidence.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-evidence-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Evidence
---
