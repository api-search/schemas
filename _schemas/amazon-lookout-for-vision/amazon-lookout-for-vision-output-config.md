---
description: The S3 location where Amazon Lookout for Vision saves model training files.
layout: schema
name: OutputConfig
properties_list:
- description: ''
  name: S3Location
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-output-config-schema.json
slug: amazon-lookout-for-vision-output-config
source_filename: amazon-lookout-for-vision-output-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-output-config-schema.json\",\n  \"title\": \"OutputConfig\",\n  \"description\": \"The S3 location where Amazon Lookout for Vision saves model training files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"The S3 location for the output.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-output-config-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: OutputConfig
---
