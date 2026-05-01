---
description: Specifies criteria for sorting the results of a query that retrieves aggregated statistical data about findings.
layout: schema
name: FindingStatisticsSortCriteria
properties_list:
- description: ''
  name: attributeName
  type: object
- description: ''
  name: orderBy
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-finding-statistics-sort-criteria-schema.json
slug: amazon-macie-finding-statistics-sort-criteria
source_filename: amazon-macie-finding-statistics-sort-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-statistics-sort-criteria-schema.json\",\n  \"title\": \"FindingStatisticsSortCriteria\",\n  \"description\": \"Specifies criteria for sorting the results of a query that retrieves aggregated statistical data about findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingStatisticsSortAttributeName\"\n        },\n        {\n          \"description\": \"The grouping to sort the results by. Valid values are: count, sort the results by the number of findings in each group of results; and, groupKey, sort the results by the name of each group of results.\"\n        }\n      ]\n    },\n    \"orderBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderBy\"\
  \n        },\n        {\n          \"description\": \"The sort order to apply to the results, based on the value for the property specified by the attributeName property. Valid values are: ASC, sort the results in ascending order; and, DESC, sort the results in descending order.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-statistics-sort-criteria-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: FindingStatisticsSortCriteria
---
