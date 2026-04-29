---
description: GetCoverageStatisticsResponse schema from Amazon GuardDuty API
layout: schema
name: GetCoverageStatisticsResponse
properties_list:
- description: ''
  name: CoverageStatistics
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-coverage-statistics-response-schema.json
slug: guardduty-get-coverage-statistics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-coverage-statistics-response-schema.json\",\n  \"title\": \"GetCoverageStatisticsResponse\",\n  \"description\": \"GetCoverageStatisticsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CoverageStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStatistics\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"coverageStatistics\"\n          },\n          \"description\": \"Represents the count aggregated by the <code>statusCode</code> and <code>resourceType</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-coverage-statistics-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetCoverageStatisticsResponse
---
