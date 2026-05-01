---
description: StartModelRequest schema from Amazon Lookout for Vision API
layout: schema
name: StartModelRequest
properties_list:
- description: ''
  name: MinInferenceUnits
  type: object
- description: ''
  name: MaxInferenceUnits
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-start-model-request-schema.json
slug: amazon-lookout-for-vision-start-model-request
source_filename: amazon-lookout-for-vision-start-model-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-start-model-request-schema.json\",\n  \"title\": \"StartModelRequest\",\n  \"description\": \"StartModelRequest schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MinInferenceUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferenceUnits\"\n        },\n        {\n          \"description\": \"The minimum number of inference units to use. A single inference unit represents 1 hour of processing. Use a higher number to increase the TPS throughput of your model. You are charged for the number of inference units that you use. \"\n        }\n      ]\n    },\n    \"MaxInferenceUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferenceUnits\"\n        },\n\
  \        {\n          \"description\": \"The maximum number of inference units to use for auto-scaling the model. If you don't specify a value, Amazon Lookout for Vision doesn't auto-scale the model.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MinInferenceUnits\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-start-model-request-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: StartModelRequest
---
