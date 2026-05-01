---
description: ListTagsForResourceResponse schema from Amazon Lookout for Vision API
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-list-tags-for-resource-response-schema.json
slug: amazon-lookout-for-vision-list-tags-for-resource-response
source_filename: amazon-lookout-for-vision-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"ListTagsForResourceResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A map of tag keys and values attached to the specified model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-list-tags-for-resource-response-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ListTagsForResourceResponse
---
