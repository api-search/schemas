---
description: Represents the reason the scan was triggered.
layout: schema
name: TriggerDetails
properties_list:
- description: ''
  name: GuardDutyFindingId
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-trigger-details-schema.json
slug: guardduty-trigger-details
source_filename: guardduty-trigger-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-trigger-details-schema.json\",\n  \"title\": \"TriggerDetails\",\n  \"description\": \"Represents the reason the scan was triggered.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GuardDutyFindingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"guardDutyFindingId\"\n          },\n          \"description\": \"The ID of the GuardDuty finding that triggered the malware scan.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"The description of the\
  \ scan trigger.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-trigger-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: TriggerDetails
---
