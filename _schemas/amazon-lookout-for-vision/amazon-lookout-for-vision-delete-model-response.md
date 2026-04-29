---
description: DeleteModelResponse schema from Amazon Lookout for Vision API
layout: schema
name: DeleteModelResponse
properties_list:
- description: ''
  name: ModelArn
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-delete-model-response-schema.json
slug: amazon-lookout-for-vision-delete-model-response
source_filename: amazon-lookout-for-vision-delete-model-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-delete-model-response-schema.json\",\n  \"title\": \"DeleteModelResponse\",\n  \"description\": \"DeleteModelResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the model that was deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-delete-model-response-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DeleteModelResponse
---
