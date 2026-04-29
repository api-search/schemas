---
description: Contains information on the sum of usage based on an Amazon Web Services resource.
layout: schema
name: UsageResourceResult
properties_list:
- description: ''
  name: Resource
  type: object
- description: ''
  name: Total
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-usage-resource-result-schema.json
slug: guardduty-usage-resource-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-resource-result-schema.json\",\n  \"title\": \"UsageResourceResult\",\n  \"description\": \"Contains information on the sum of usage based on an Amazon Web Services resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resource\"\n          },\n          \"description\": \"The Amazon Web Services resource that generated usage.\"\n        }\n      ]\n    },\n    \"Total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Total\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"total\"\n          },\n          \"description\": \"Represents the sum total of usage\
  \ for the specified resource type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-usage-resource-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UsageResourceResult
---
