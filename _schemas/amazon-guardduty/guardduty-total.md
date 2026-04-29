---
description: Contains the total usage with the corresponding currency unit for that value.
layout: schema
name: Total
properties_list:
- description: ''
  name: Amount
  type: object
- description: ''
  name: Unit
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-total-schema.json
slug: guardduty-total
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-total-schema.json\",\n  \"title\": \"Total\",\n  \"description\": \"Contains the total usage with the corresponding currency unit for that value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Amount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"amount\"\n          },\n          \"description\": \"The total usage.\"\n        }\n      ]\n    },\n    \"Unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"unit\"\n          },\n          \"description\": \"The currency unit that the amount is given in.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-total-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Total
---
