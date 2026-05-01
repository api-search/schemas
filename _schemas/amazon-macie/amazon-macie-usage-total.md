---
description: Provides aggregated data for an Amazon Macie usage metric. The value for the metric reports estimated usage data for an account for the preceding 30 days or the current calendar month to date, depending on the time period (timeRange) specified in the request.
layout: schema
name: UsageTotal
properties_list:
- description: ''
  name: currency
  type: object
- description: ''
  name: estimatedCost
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-usage-total-schema.json
slug: amazon-macie-usage-total
source_filename: amazon-macie-usage-total-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-usage-total-schema.json\",\n  \"title\": \"UsageTotal\",\n  \"description\": \"Provides aggregated data for an Amazon Macie usage metric. The value for the metric reports estimated usage data for an account for the preceding 30 days or the current calendar month to date, depending on the time period (timeRange) specified in the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Currency\"\n        },\n        {\n          \"description\": \"The type of currency that the value for the metric (estimatedCost) is reported in.\"\n        }\n      ]\n    },\n    \"estimatedCost\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n     \
  \     \"description\": \"The estimated value for the metric.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageType\"\n        },\n        {\n          \"description\": \"The name of the metric. Possible values are: AUTOMATED_OBJECT_MONITORING, to monitor S3 objects for automated sensitive data discovery; AUTOMATED_SENSITIVE_DATA_DISCOVERY, to analyze S3 objects for automated sensitive data discovery; DATA_INVENTORY_EVALUATION, to monitor S3 buckets; and, SENSITIVE_DATA_DISCOVERY, to run classification jobs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-usage-total-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UsageTotal
---
