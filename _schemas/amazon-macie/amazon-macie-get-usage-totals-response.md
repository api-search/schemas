---
description: GetUsageTotalsResponse schema from Amazon Macie API
layout: schema
name: GetUsageTotalsResponse
properties_list:
- description: ''
  name: timeRange
  type: object
- description: ''
  name: usageTotals
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-usage-totals-response-schema.json
slug: amazon-macie-get-usage-totals-response
source_filename: amazon-macie-get-usage-totals-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-usage-totals-response-schema.json\",\n  \"title\": \"GetUsageTotalsResponse\",\n  \"description\": \"GetUsageTotalsResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timeRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeRange\"\n        },\n        {\n          \"description\": \"The inclusive time period that the usage data applies to. Possible values are: MONTH_TO_DATE, for the current calendar month to date; and, PAST_30_DAYS, for the preceding 30 days.\"\n        }\n      ]\n    },\n    \"usageTotals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfUsageTotal\"\n        },\n        {\n          \"description\": \"An array of objects that contains the results of the\
  \ query. Each object contains the data for a specific usage metric.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-usage-totals-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetUsageTotalsResponse
---
