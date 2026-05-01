---
description: CreateModelRequest schema from Amazon Lookout for Vision API
layout: schema
name: CreateModelRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: OutputConfig
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-create-model-request-schema.json
slug: amazon-lookout-for-vision-create-model-request
source_filename: amazon-lookout-for-vision-create-model-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-create-model-request-schema.json\",\n  \"title\": \"CreateModelRequest\",\n  \"description\": \"CreateModelRequest schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelDescriptionMessage\"\n        },\n        {\n          \"description\": \"A description for the version of the model.\"\n        }\n      ]\n    },\n    \"OutputConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputConfig\"\n        },\n        {\n          \"description\": \"The location where Amazon Lookout for Vision saves the training results.\"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"The identifier for your AWS KMS key. The key is used to encrypt training and test images copied into the service for model training. Your source images are unaffected. If this parameter is not specified, the copied images are encrypted by a key that AWS owns and manages.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A set of tags (key-value pairs) that you want to attach to the model.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OutputConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-create-model-request-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: CreateModelRequest
---
