---
description: A list of tag key and value pairs that you define.
layout: schema
name: Tag
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-tag-schema.json
slug: compute-optimizer-tag
source_filename: compute-optimizer-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \" A list of tag key and value pairs that you define. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \" One part of a key-value pair that makes up a tag. A key is a general label that acts like a category for more specific tag values. \"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \" One part of a key-value pair that make up a tag. A value acts as a descriptor within a tag category (key). The value can be empty or null. \"\n  \
  \      }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-tag-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: Tag
---
