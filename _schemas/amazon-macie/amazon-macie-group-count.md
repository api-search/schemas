---
description: Provides a group of results for a query that retrieved aggregated statistical data about findings.
layout: schema
name: GroupCount
properties_list:
- description: ''
  name: count
  type: object
- description: ''
  name: groupKey
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-group-count-schema.json
slug: amazon-macie-group-count
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-group-count-schema.json\",\n  \"title\": \"GroupCount\",\n  \"description\": \"Provides a group of results for a query that retrieved aggregated statistical data about findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of findings in the group of query results.\"\n        }\n      ]\n    },\n    \"groupKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the property that defines the group in the query results, as specified by the groupBy property in the query request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-group-count-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GroupCount
---
