---
description: Represents the result of the scan.
layout: schema
name: ScanResultDetails
properties_list:
- description: ''
  name: ScanResult
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-result-details-schema.json
slug: guardduty-scan-result-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-result-details-schema.json\",\n  \"title\": \"ScanResultDetails\",\n  \"description\": \"Represents the result of the scan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScanResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanResult\"\n          },\n          \"description\": \"An enum value representing possible scan results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-result-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanResultDetails
---
