---
description: Specifies criteria for sorting the results of a request for information about classification jobs.
layout: schema
name: ListJobsSortCriteria
properties_list:
- description: ''
  name: attributeName
  type: object
- description: ''
  name: orderBy
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-list-jobs-sort-criteria-schema.json
slug: amazon-macie-list-jobs-sort-criteria
source_filename: amazon-macie-list-jobs-sort-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-jobs-sort-criteria-schema.json\",\n  \"title\": \"ListJobsSortCriteria\",\n  \"description\": \"Specifies criteria for sorting the results of a request for information about classification jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListJobsSortAttributeName\"\n        },\n        {\n          \"description\": \"The property to sort the results by.\"\n        }\n      ]\n    },\n    \"orderBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderBy\"\n        },\n        {\n          \"description\": \"The sort order to apply to the results, based on the value for the property specified by the attributeName property. Valid values are: ASC, sort the\
  \ results in ascending order; and, DESC, sort the results in descending order.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-jobs-sort-criteria-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListJobsSortCriteria
---
