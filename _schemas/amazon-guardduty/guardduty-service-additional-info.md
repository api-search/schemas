---
description: Additional information about the generated finding.
layout: schema
name: ServiceAdditionalInfo
properties_list:
- description: ''
  name: Value
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-service-additional-info-schema.json
slug: guardduty-service-additional-info
source_filename: guardduty-service-additional-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-service-additional-info-schema.json\",\n  \"title\": \"ServiceAdditionalInfo\",\n  \"description\": \"Additional information about the generated finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"value\"\n          },\n          \"description\": \"This field specifies the value of the additional information.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"Describes the type of the additional information.\"\n       \
  \ }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-service-additional-info-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ServiceAdditionalInfo
---
