---
description: CreateIPSetResponse schema from Amazon GuardDuty API
layout: schema
name: CreateIPSetResponse
properties_list:
- description: ''
  name: IpSetId
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-create-ip-set-response-schema.json
slug: guardduty-create-ip-set-response
source_filename: guardduty-create-ip-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-ip-set-response-schema.json\",\n  \"title\": \"CreateIPSetResponse\",\n  \"description\": \"CreateIPSetResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ipSetId\"\n          },\n          \"description\": \"The ID of the IPSet resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IpSetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-ip-set-response-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CreateIPSetResponse
---
