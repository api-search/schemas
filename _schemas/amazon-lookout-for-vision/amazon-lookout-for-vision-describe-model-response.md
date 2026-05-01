---
description: DescribeModelResponse schema from Amazon Lookout for Vision API
layout: schema
name: DescribeModelResponse
properties_list:
- description: ''
  name: ModelDescription
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-describe-model-response-schema.json
slug: amazon-lookout-for-vision-describe-model-response
source_filename: amazon-lookout-for-vision-describe-model-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-describe-model-response-schema.json\",\n  \"title\": \"DescribeModelResponse\",\n  \"description\": \"DescribeModelResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModelDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelDescription\"\n        },\n        {\n          \"description\": \"Contains the description of the model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-describe-model-response-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DescribeModelResponse
---
