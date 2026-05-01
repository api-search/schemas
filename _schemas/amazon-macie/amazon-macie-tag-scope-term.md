---
description: Specifies a tag-based condition that determines whether an S3 object is included or excluded from a classification job.
layout: schema
name: TagScopeTerm
properties_list:
- description: ''
  name: comparator
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: tagValues
  type: object
- description: ''
  name: target
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-tag-scope-term-schema.json
slug: amazon-macie-tag-scope-term
source_filename: amazon-macie-tag-scope-term-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-tag-scope-term-schema.json\",\n  \"title\": \"TagScopeTerm\",\n  \"description\": \"Specifies a tag-based condition that determines whether an S3 object is included or excluded from a classification job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobComparator\"\n        },\n        {\n          \"description\": \"The operator to use in the condition. Valid values are EQ (equals) or NE (not equals).\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The object property to use in the condition. The only valid value is TAG.\"\n        }\n      ]\n    },\n    \"\
  tagValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfTagValuePair\"\n        },\n        {\n          \"description\": \"The tag keys or tag key and value pairs to use in the condition. To specify only tag keys in a condition, specify the keys in this array and set the value for each associated tag value to an empty string.\"\n        }\n      ]\n    },\n    \"target\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagTarget\"\n        },\n        {\n          \"description\": \"The type of object to apply the condition to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-tag-scope-term-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: TagScopeTerm
---
