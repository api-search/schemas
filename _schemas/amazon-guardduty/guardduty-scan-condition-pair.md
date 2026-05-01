---
description: Represents key, value pair to be matched against given resource property.
layout: schema
name: ScanConditionPair
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-condition-pair-schema.json
slug: guardduty-scan-condition-pair
source_filename: guardduty-scan-condition-pair-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-condition-pair-schema.json\",\n  \"title\": \"ScanConditionPair\",\n  \"description\": \"Represents key, value pair to be matched against given resource property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"key\"\n          },\n          \"description\": \"Represents <i>key</i> <b/> in the map condition.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"value\"\n          },\n          \"description\": \"Represents optional <i>value</i> <b/> in the map condition.\
  \ If not specified, only <i>key</i> <b/> will be matched.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-condition-pair-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanConditionPair
---
