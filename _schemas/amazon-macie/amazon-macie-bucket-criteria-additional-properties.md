---
description: Specifies the operator to use in a property-based condition that filters the results of a query for information about S3 buckets.
layout: schema
name: BucketCriteriaAdditionalProperties
properties_list:
- description: ''
  name: eq
  type: object
- description: ''
  name: gt
  type: object
- description: ''
  name: gte
  type: object
- description: ''
  name: lt
  type: object
- description: ''
  name: lte
  type: object
- description: ''
  name: neq
  type: object
- description: ''
  name: prefix
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-criteria-additional-properties-schema.json
slug: amazon-macie-bucket-criteria-additional-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-criteria-additional-properties-schema.json\",\n  \"title\": \"BucketCriteriaAdditionalProperties\",\n  \"description\": \"Specifies the operator to use in a property-based condition that filters the results of a query for information about S3 buckets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eq\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"The value for the property matches (equals) the specified value. If you specify multiple values, Amazon Macie uses OR logic to join the values.\"\n        }\n      ]\n    },\n    \"gt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The value\
  \ for the property is greater than the specified value.\"\n        }\n      ]\n    },\n    \"gte\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The value for the property is greater than or equal to the specified value.\"\n        }\n      ]\n    },\n    \"lt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The value for the property is less than the specified value.\"\n        }\n      ]\n    },\n    \"lte\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The value for the property is less than or equal to the specified value.\"\n        }\n      ]\n    },\n    \"neq\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\"\
  : \"The value for the property doesn't match (doesn't equal) the specified value. If you specify multiple values, Amazon Macie uses OR logic to join the values.\"\n        }\n      ]\n    },\n    \"prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the bucket begins with the specified value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-criteria-additional-properties-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketCriteriaAdditionalProperties
---
