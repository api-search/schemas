---
description: Specifies property- and tag-based conditions that define filter criteria for including or excluding S3 buckets from the query results. Exclude conditions take precedence over include conditions.
layout: schema
name: SearchResourcesBucketCriteria
properties_list:
- description: ''
  name: excludes
  type: object
- description: ''
  name: includes
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-search-resources-bucket-criteria-schema.json
slug: amazon-macie-search-resources-bucket-criteria
source_filename: amazon-macie-search-resources-bucket-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-bucket-criteria-schema.json\",\n  \"title\": \"SearchResourcesBucketCriteria\",\n  \"description\": \"Specifies property- and tag-based conditions that define filter criteria for including or excluding S3 buckets from the query results. Exclude conditions take precedence over include conditions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excludes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchResourcesCriteriaBlock\"\n        },\n        {\n          \"description\": \"The property- and tag-based conditions that determine which buckets to exclude from the results.\"\n        }\n      ]\n    },\n    \"includes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchResourcesCriteriaBlock\"\n    \
  \    },\n        {\n          \"description\": \"The property- and tag-based conditions that determine which buckets to include in the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-bucket-criteria-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SearchResourcesBucketCriteria
---
