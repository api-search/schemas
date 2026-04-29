---
description: CreateSampleFindingsRequest schema from Amazon GuardDuty API
layout: schema
name: CreateSampleFindingsRequest
properties_list:
- description: ''
  name: FindingTypes
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-create-sample-findings-request-schema.json
slug: guardduty-create-sample-findings-request
source_filename: guardduty-create-sample-findings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-sample-findings-request-schema.json\",\n  \"title\": \"CreateSampleFindingsRequest\",\n  \"description\": \"CreateSampleFindingsRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FindingTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingTypes\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingTypes\"\n          },\n          \"description\": \"The types of sample findings to generate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-sample-findings-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CreateSampleFindingsRequest
---
