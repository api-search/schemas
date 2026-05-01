---
description: Contains list of scanned and skipped EBS volumes with details.
layout: schema
name: EbsVolumeDetails
properties_list:
- description: ''
  name: ScannedVolumeDetails
  type: object
- description: ''
  name: SkippedVolumeDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-ebs-volume-details-schema.json
slug: guardduty-ebs-volume-details
source_filename: guardduty-ebs-volume-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ebs-volume-details-schema.json\",\n  \"title\": \"EbsVolumeDetails\",\n  \"description\": \"Contains list of scanned and skipped EBS volumes with details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScannedVolumeDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scannedVolumeDetails\"\n          },\n          \"description\": \"List of EBS volumes that were scanned.\"\n        }\n      ]\n    },\n    \"SkippedVolumeDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"skippedVolumeDetails\"\n          },\n          \"description\": \"List of\
  \ EBS volumes that were skipped from the malware scan.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ebs-volume-details-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: EbsVolumeDetails
---
