---
description: GetUsageStatisticsRequest schema from Amazon Macie API
layout: schema
name: GetUsageStatisticsRequest
properties_list:
- description: ''
  name: filterBy
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: timeRange
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-usage-statistics-request-schema.json
slug: amazon-macie-get-usage-statistics-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-usage-statistics-request-schema.json\",\n  \"title\": \"GetUsageStatisticsRequest\",\n  \"description\": \"GetUsageStatisticsRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filterBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfUsageStatisticsFilter\"\n        },\n        {\n          \"description\": \"An array of objects, one for each condition to use to filter the query results. If you specify more than one condition, Amazon Macie uses an AND operator to join the conditions.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of items to include\
  \ in each page of the response.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The nextToken string that specifies which page of results to return in a paginated response.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageStatisticsSortBy\"\n        },\n        {\n          \"description\": \"The criteria to use to sort the query results.\"\n        }\n      ]\n    },\n    \"timeRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeRange\"\n        },\n        {\n          \"description\": \"The inclusive time period to query usage data for. Valid values are: MONTH_TO_DATE, for the current calendar month to date; and, PAST_30_DAYS, for the preceding 30 days. If you don't specify a value, Amazon Macie provides usage data for the preceding\
  \ 30 days.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-usage-statistics-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetUsageStatisticsRequest
---
