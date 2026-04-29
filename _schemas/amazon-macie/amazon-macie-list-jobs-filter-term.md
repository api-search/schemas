---
description: Specifies a condition that filters the results of a request for information about classification jobs. Each condition consists of a property, an operator, and one or more values.
layout: schema
name: ListJobsFilterTerm
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
schema_file: json-schema/amazon-macie-list-jobs-filter-term-schema.json
slug: amazon-macie-list-jobs-filter-term
source_filename: amazon-macie-list-jobs-filter-term-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-jobs-filter-term-schema.json\",\n  \"title\": \"ListJobsFilterTerm\",\n  \"description\": \"Specifies a condition that filters the results of a request for information about classification jobs. Each condition consists of a property, an operator, and one or more values.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobComparator\"\n        },\n        {\n          \"description\": \"The operator to use to filter the results.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListJobsFilterKey\"\n        },\n        {\n          \"description\": \"The property to use to filter the results.\"\n        }\n      ]\n    },\n\
  \    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array that lists one or more values to use to filter the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-jobs-filter-term-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListJobsFilterTerm
---
