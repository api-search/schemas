---
description: Specifies a condition for filtering the results of a query for quota and usage data for one or more Amazon Macie accounts.
layout: schema
name: UsageStatisticsFilter
properties_list:
- description: ''
  name: comparator
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-usage-statistics-filter-schema.json
slug: amazon-macie-usage-statistics-filter
source_filename: amazon-macie-usage-statistics-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-usage-statistics-filter-schema.json\",\n  \"title\": \"UsageStatisticsFilter\",\n  \"description\": \"Specifies a condition for filtering the results of a query for quota and usage data for one or more Amazon Macie accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageStatisticsFilterComparator\"\n        },\n        {\n          \"description\": \"The operator to use in the condition. If the value for the key property is accountId, this value must be CONTAINS. If the value for the key property is any other supported field, this value can be EQ, GT, GTE, LT, LTE, or NE.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageStatisticsFilterKey\"\
  \n        },\n        {\n          \"description\": \"The field to use in the condition.\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"<p>An array that lists values to use in the condition, based on the value for the field specified by the key property. If the value for the key property is accountId, this array can specify multiple values. Otherwise, this array can specify only one value.</p> <p>Valid values for each supported field are:</p> <ul><li><p>accountId - The unique identifier for an Amazon Web Services account.</p></li> <li><p>freeTrialStartDate - The date and time, in UTC and extended ISO 8601 format, when the Amazon Macie free trial started for an account.</p></li> <li><p>serviceLimit - A Boolean (true or false) value that indicates whether an account has reached its monthly quota.</p></li> <li><p>total - A string that represents\
  \ the current estimated cost for an account.</p></li></ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-usage-statistics-filter-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UsageStatisticsFilter
---
