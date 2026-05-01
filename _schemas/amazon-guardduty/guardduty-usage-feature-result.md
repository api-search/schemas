---
description: Contains information about the result of the total usage based on the feature.
layout: schema
name: UsageFeatureResult
properties_list:
- description: ''
  name: Feature
  type: object
- description: ''
  name: Total
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-usage-feature-result-schema.json
slug: guardduty-usage-feature-result
source_filename: guardduty-usage-feature-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-feature-result-schema.json\",\n  \"title\": \"UsageFeatureResult\",\n  \"description\": \"Contains information about the result of the total usage based on the feature.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Feature\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageFeature\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"feature\"\n          },\n          \"description\": \"The feature that generated the usage cost.\"\n        }\n      ]\n    },\n    \"Total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Total\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"total\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-feature-result-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UsageFeatureResult
---
