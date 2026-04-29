---
description: GetUsageStatisticsRequest schema from Amazon GuardDuty API
layout: schema
name: GetUsageStatisticsRequest
properties_list:
- description: ''
  name: UsageStatisticType
  type: object
- description: ''
  name: UsageCriteria
  type: object
- description: ''
  name: Unit
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-usage-statistics-request-schema.json
slug: guardduty-get-usage-statistics-request
source_filename: guardduty-get-usage-statistics-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-usage-statistics-request-schema.json\",\n  \"title\": \"GetUsageStatisticsRequest\",\n  \"description\": \"GetUsageStatisticsRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UsageStatisticType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageStatisticType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"usageStatisticsType\"\n          },\n          \"description\": \"The type of usage statistics to retrieve.\"\n        }\n      ]\n    },\n    \"UsageCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageCriteria\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"usageCriteria\"\n          },\n          \"description\": \"\
  Represents the criteria used for querying usage.\"\n        }\n      ]\n    },\n    \"Unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"unit\"\n          },\n          \"description\": \"The currency unit you would like to view your usage statistics in. Current valid values are USD.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxResults\"\n          },\n          \"description\": \"The maximum number of results to return in the response.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"A token to use\
  \ for paginating results that are returned in the response. Set the value of this parameter to null for the first request to a list action. For subsequent calls, use the NextToken value returned from the previous request to continue listing results after the first page.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UsageStatisticType\",\n    \"UsageCriteria\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-usage-statistics-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetUsageStatisticsRequest
---
