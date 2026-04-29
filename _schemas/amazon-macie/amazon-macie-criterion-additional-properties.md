---
description: Specifies the operator to use in a property-based condition that filters the results of a query for findings. For detailed information and examples of each operator, see <a href="https://docs.aws.amazon.com/macie/latest/user/findings-filter-basics.html">Fundamentals of filtering findings</a> in the <i>Amazon Macie User Guide</i>.
layout: schema
name: CriterionAdditionalProperties
properties_list:
- description: ''
  name: eq
  type: object
- description: ''
  name: eqExactMatch
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
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-criterion-additional-properties-schema.json
slug: amazon-macie-criterion-additional-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-criterion-additional-properties-schema.json\",\n  \"title\": \"CriterionAdditionalProperties\",\n  \"description\": \"Specifies the operator to use in a property-based condition that filters the results of a query for findings. For detailed information and examples of each operator, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/findings-filter-basics.html\\\">Fundamentals of filtering findings</a> in the <i>Amazon Macie User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eq\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"The value for the property matches (equals) the specified value. If you specify multiple values, Macie uses OR logic to join the values.\"\
  \n        }\n      ]\n    },\n    \"eqExactMatch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"<p>The value for the property exclusively matches (equals an exact match for) all the specified values. If you specify multiple values, Amazon Macie uses AND logic to join the values.</p> <p>You can use this operator with the following properties: customDataIdentifiers.detections.arn, customDataIdentifiers.detections.name, resourcesAffected.s3Bucket.tags.key, resourcesAffected.s3Bucket.tags.value, resourcesAffected.s3Object.tags.key, resourcesAffected.s3Object.tags.value, sensitiveData.category, and sensitiveData.detections.type.</p>\"\n        }\n      ]\n    },\n    \"gt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The value for the property is greater than the specified value.\"\n        }\n\
  \      ]\n    },\n    \"gte\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The value for the property is greater than or equal to the specified value.\"\n        }\n      ]\n    },\n    \"lt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The value for the property is less than the specified value.\"\n        }\n      ]\n    },\n    \"lte\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The value for the property is less than or equal to the specified value.\"\n        }\n      ]\n    },\n    \"neq\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"The value for the property doesn't match (doesn't equal) the specified\
  \ value. If you specify multiple values, Macie uses OR logic to join the values.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-criterion-additional-properties-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CriterionAdditionalProperties
---
