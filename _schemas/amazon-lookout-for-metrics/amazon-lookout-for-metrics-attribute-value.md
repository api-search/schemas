---
description: An attribute value.
layout: schema
name: AttributeValue
properties_list:
- description: ''
  name: S
  type: object
- description: ''
  name: N
  type: object
- description: ''
  name: B
  type: object
- description: ''
  name: SS
  type: object
- description: ''
  name: NS
  type: object
- description: ''
  name: BS
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-attribute-value-schema.json
slug: amazon-lookout-for-metrics-attribute-value
source_filename: amazon-lookout-for-metrics-attribute-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-attribute-value-schema.json\",\n  \"title\": \"AttributeValue\",\n  \"description\": \"An attribute value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringAttributeValue\"\n        },\n        {\n          \"description\": \"A string.\"\n        }\n      ]\n    },\n    \"N\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberAttributeValue\"\n        },\n        {\n          \"description\": \"A number.\"\n        }\n      ]\n    },\n    \"B\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BinaryAttributeValue\"\n        },\n        {\n          \"description\": \"A binary value.\"\n        }\n      ]\n    },\n\
  \    \"SS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringListAttributeValue\"\n        },\n        {\n          \"description\": \"A list of strings.\"\n        }\n      ]\n    },\n    \"NS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberListAttributeValue\"\n        },\n        {\n          \"description\": \"A list of numbers.\"\n        }\n      ]\n    },\n    \"BS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BinaryListAttributeValue\"\n        },\n        {\n          \"description\": \"A list of binary values.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-attribute-value-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AttributeValue
---
