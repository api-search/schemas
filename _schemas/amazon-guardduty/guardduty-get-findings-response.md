---
description: GetFindingsResponse schema from Amazon GuardDuty API
layout: schema
name: GetFindingsResponse
properties_list:
- description: ''
  name: Findings
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-findings-response-schema.json
slug: guardduty-get-findings-response
source_filename: guardduty-get-findings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-findings-response-schema.json\",\n  \"title\": \"GetFindingsResponse\",\n  \"description\": \"GetFindingsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Findings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Findings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findings\"\n          },\n          \"description\": \"A list of findings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Findings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-findings-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetFindingsResponse
---
