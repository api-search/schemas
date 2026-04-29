---
description: GetFindingsRequest schema from Amazon Macie API
layout: schema
name: GetFindingsRequest
properties_list:
- description: ''
  name: findingIds
  type: object
- description: ''
  name: sortCriteria
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-findings-request-schema.json
slug: amazon-macie-get-findings-request
source_filename: amazon-macie-get-findings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-findings-request-schema.json\",\n  \"title\": \"GetFindingsRequest\",\n  \"description\": \"GetFindingsRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of strings that lists the unique identifiers for the findings to retrieve. You can specify as many as 50 unique identifiers in this array.\"\n        }\n      ]\n    },\n    \"sortCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortCriteria\"\n        },\n        {\n          \"description\": \"The criteria for sorting the results of the request.\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"findingIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-findings-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetFindingsRequest
---
