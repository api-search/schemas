---
description: Contains information about criteria used to filter resources before triggering malware scan.
layout: schema
name: ScanResourceCriteria
properties_list:
- description: ''
  name: Include
  type: object
- description: ''
  name: Exclude
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-resource-criteria-schema.json
slug: guardduty-scan-resource-criteria
source_filename: guardduty-scan-resource-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-resource-criteria-schema.json\",\n  \"title\": \"ScanResourceCriteria\",\n  \"description\": \"Contains information about criteria used to filter resources before triggering malware scan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Include\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanCriterion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"include\"\n          },\n          \"description\": \"Represents condition that when matched will allow a malware scan for a certain resource.\"\n        }\n      ]\n    },\n    \"Exclude\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanCriterion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"exclude\"\n          },\n\
  \          \"description\": \"Represents condition that when matched will prevent a malware scan for a certain resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-resource-criteria-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanResourceCriteria
---
