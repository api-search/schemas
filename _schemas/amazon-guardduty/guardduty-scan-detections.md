---
description: Contains a complete view providing malware scan result details.
layout: schema
name: ScanDetections
properties_list:
- description: ''
  name: ScannedItemCount
  type: object
- description: ''
  name: ThreatsDetectedItemCount
  type: object
- description: ''
  name: HighestSeverityThreatDetails
  type: object
- description: ''
  name: ThreatDetectedByName
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-detections-schema.json
slug: guardduty-scan-detections
source_filename: guardduty-scan-detections-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-detections-schema.json\",\n  \"title\": \"ScanDetections\",\n  \"description\": \"Contains a complete view providing malware scan result details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScannedItemCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScannedItemCount\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scannedItemCount\"\n          },\n          \"description\": \"Total number of scanned files.\"\n        }\n      ]\n    },\n    \"ThreatsDetectedItemCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThreatsDetectedItemCount\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"threatsDetectedItemCount\"\n          },\n          \"description\": \"Total\
  \ number of infected files.\"\n        }\n      ]\n    },\n    \"HighestSeverityThreatDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HighestSeverityThreatDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"highestSeverityThreatDetails\"\n          },\n          \"description\": \"Details of the highest severity threat detected during malware scan and number of infected files.\"\n        }\n      ]\n    },\n    \"ThreatDetectedByName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThreatDetectedByName\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"threatDetectedByName\"\n          },\n          \"description\": \"Contains details about identified threats organized by threat name.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-detections-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanDetections
---
