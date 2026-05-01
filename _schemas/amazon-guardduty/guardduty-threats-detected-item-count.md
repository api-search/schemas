---
description: Contains total number of infected files.
layout: schema
name: ThreatsDetectedItemCount
properties_list:
- description: ''
  name: Files
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-threats-detected-item-count-schema.json
slug: guardduty-threats-detected-item-count
source_filename: guardduty-threats-detected-item-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-threats-detected-item-count-schema.json\",\n  \"title\": \"ThreatsDetectedItemCount\",\n  \"description\": \"Contains total number of infected files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Files\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"files\"\n          },\n          \"description\": \"Total number of infected files.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-threats-detected-item-count-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ThreatsDetectedItemCount
---
