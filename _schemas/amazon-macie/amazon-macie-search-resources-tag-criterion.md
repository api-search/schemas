---
description: Specifies a tag-based filter condition that determines which Amazon Web Services resources are included or excluded from the query results.
layout: schema
name: SearchResourcesTagCriterion
properties_list:
- description: ''
  name: comparator
  type: object
- description: ''
  name: tagValues
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-search-resources-tag-criterion-schema.json
slug: amazon-macie-search-resources-tag-criterion
source_filename: amazon-macie-search-resources-tag-criterion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-tag-criterion-schema.json\",\n  \"title\": \"SearchResourcesTagCriterion\",\n  \"description\": \"Specifies a tag-based filter condition that determines which Amazon Web Services resources are included or excluded from the query results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchResourcesComparator\"\n        },\n        {\n          \"description\": \"The operator to use in the condition. Valid values are EQ (equals) and NE (not equals).\"\n        }\n      ]\n    },\n    \"tagValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSearchResourcesTagCriterionPair\"\n        },\n        {\n          \"description\": \"The tag keys,\
  \ tag values, or tag key and value pairs to use in the condition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-tag-criterion-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SearchResourcesTagCriterion
---
