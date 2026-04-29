---
description: StopModelResponse schema from Amazon Lookout for Vision API
layout: schema
name: StopModelResponse
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-stop-model-response-schema.json
slug: amazon-lookout-for-vision-stop-model-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-stop-model-response-schema.json\",\n  \"title\": \"StopModelResponse\",\n  \"description\": \"StopModelResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelHostingStatus\"\n        },\n        {\n          \"description\": \"The status of the model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-stop-model-response-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: StopModelResponse
---
