---
description: Contains information about the condition.
layout: schema
name: ScanCondition
properties_list:
- description: ''
  name: MapEquals
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-condition-schema.json
slug: guardduty-scan-condition
source_filename: guardduty-scan-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-condition-schema.json\",\n  \"title\": \"ScanCondition\",\n  \"description\": \"Contains information about the condition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MapEquals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapEquals\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mapEquals\"\n          },\n          \"description\": \"Represents an <i>mapEqual</i> <b/> condition to be applied to a single field when triggering for malware scan.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MapEquals\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-condition-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanCondition
---
