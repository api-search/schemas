---
description: Contains details from the malware scan that created a finding.
layout: schema
name: EbsVolumeScanDetails
properties_list:
- description: ''
  name: ScanId
  type: object
- description: ''
  name: ScanStartedAt
  type: object
- description: ''
  name: ScanCompletedAt
  type: object
- description: ''
  name: TriggerFindingId
  type: object
- description: ''
  name: Sources
  type: object
- description: ''
  name: ScanDetections
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-ebs-volume-scan-details-schema.json
slug: guardduty-ebs-volume-scan-details
source_filename: guardduty-ebs-volume-scan-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ebs-volume-scan-details-schema.json\",\n  \"title\": \"EbsVolumeScanDetails\",\n  \"description\": \"Contains details from the malware scan that created a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScanId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanId\"\n          },\n          \"description\": \"Unique Id of the malware scan that generated the finding.\"\n        }\n      ]\n    },\n    \"ScanStartedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanStartedAt\"\n          },\n          \"description\": \"Returns the start date and time\
  \ of the malware scan.\"\n        }\n      ]\n    },\n    \"ScanCompletedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanCompletedAt\"\n          },\n          \"description\": \"Returns the completion date and time of the malware scan.\"\n        }\n      ]\n    },\n    \"TriggerFindingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"triggerFindingId\"\n          },\n          \"description\": \"GuardDuty finding ID that triggered a malware scan.\"\n        }\n      ]\n    },\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Sources\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          },\n          \"description\": \"Contains list of threat intelligence sources used to detect\
  \ threats.\"\n        }\n      ]\n    },\n    \"ScanDetections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanDetections\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanDetections\"\n          },\n          \"description\": \"Contains a complete view providing malware scan result details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ebs-volume-scan-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: EbsVolumeScanDetails
---
