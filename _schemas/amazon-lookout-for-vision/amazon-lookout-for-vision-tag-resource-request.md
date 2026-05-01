---
description: TagResourceRequest schema from Amazon Lookout for Vision API
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-tag-resource-request-schema.json
slug: amazon-lookout-for-vision-tag-resource-request
source_filename: amazon-lookout-for-vision-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The key-value tags to assign to the model.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-tag-resource-request-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: TagResourceRequest
---
