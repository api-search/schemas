---
description: GetUsageStatisticsResponse schema from Amazon Macie API
layout: schema
name: GetUsageStatisticsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: records
  type: object
- description: ''
  name: timeRange
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-usage-statistics-response-schema.json
slug: amazon-macie-get-usage-statistics-response
source_filename: amazon-macie-get-usage-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-usage-statistics-response-schema.json\",\n  \"title\": \"GetUsageStatisticsResponse\",\n  \"description\": \"GetUsageStatisticsResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are no additional pages.\"\n        }\n      ]\n    },\n    \"records\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfUsageRecord\"\n        },\n        {\n          \"description\": \"An array of objects that contains the results of the query. Each object\
  \ contains the data for an account that matches the filter criteria specified in the request.\"\n        }\n      ]\n    },\n    \"timeRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeRange\"\n        },\n        {\n          \"description\": \"The inclusive time period that the usage data applies to. Possible values are: MONTH_TO_DATE, for the current calendar month to date; and, PAST_30_DAYS, for the preceding 30 days.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-usage-statistics-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetUsageStatisticsResponse
---
