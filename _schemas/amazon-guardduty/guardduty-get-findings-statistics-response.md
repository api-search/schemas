---
description: GetFindingsStatisticsResponse schema from Amazon GuardDuty API
layout: schema
name: GetFindingsStatisticsResponse
properties_list:
- description: ''
  name: FindingStatistics
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-findings-statistics-response-schema.json
slug: guardduty-get-findings-statistics-response
source_filename: guardduty-get-findings-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-findings-statistics-response-schema.json\",\n  \"title\": \"GetFindingsStatisticsResponse\",\n  \"description\": \"GetFindingsStatisticsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FindingStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingStatistics\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingStatistics\"\n          },\n          \"description\": \"The finding statistics object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FindingStatistics\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-findings-statistics-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetFindingsStatisticsResponse
---
