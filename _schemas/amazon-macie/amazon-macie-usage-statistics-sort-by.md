---
description: Specifies criteria for sorting the results of a query for Amazon Macie account quotas and usage data.
layout: schema
name: UsageStatisticsSortBy
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: orderBy
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-usage-statistics-sort-by-schema.json
slug: amazon-macie-usage-statistics-sort-by
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-usage-statistics-sort-by-schema.json\",\n  \"title\": \"UsageStatisticsSortBy\",\n  \"description\": \"Specifies criteria for sorting the results of a query for Amazon Macie account quotas and usage data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsageStatisticsSortKey\"\n        },\n        {\n          \"description\": \"The field to sort the results by.\"\n        }\n      ]\n    },\n    \"orderBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderBy\"\n        },\n        {\n          \"description\": \"The sort order to apply to the results, based on the value for the field specified by the key property. Valid values are: ASC, sort the results in ascending order;\
  \ and, DESC, sort the results in descending order.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-usage-statistics-sort-by-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UsageStatisticsSortBy
---
