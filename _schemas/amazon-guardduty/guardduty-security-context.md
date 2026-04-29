---
description: Container security context.
layout: schema
name: SecurityContext
properties_list:
- description: ''
  name: Privileged
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-security-context-schema.json
slug: guardduty-security-context
source_filename: guardduty-security-context-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-security-context-schema.json\",\n  \"title\": \"SecurityContext\",\n  \"description\": \"Container security context.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Privileged\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"privileged\"\n          },\n          \"description\": \"Whether the container is privileged.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-security-context-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: SecurityContext
---
