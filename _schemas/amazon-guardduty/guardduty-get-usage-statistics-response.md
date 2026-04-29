---
description: GetUsageStatisticsResponse schema from Amazon GuardDuty API
layout: schema
name: GetUsageStatisticsResponse
properties_list:
- description: ''
  name: UsageStatistics
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-usage-statistics-response-schema.json
slug: guardduty-get-usage-statistics-response
source_filename: guardduty-get-usage-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-usage-statistics-response-schema.json\",\n  \"title\": \"GetUsageStatisticsResponse\",\n  \"description\": \"GetUsageStatisticsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UsageStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageStatistics\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"usageStatistics\"\n          },\n          \"description\": \"The usage statistics object. If a UsageStatisticType was provided, the objects representing other types will be null.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\
  \n          },\n          \"description\": \"The pagination parameter to be used on the next list operation to retrieve more items.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-usage-statistics-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetUsageStatisticsResponse
---
