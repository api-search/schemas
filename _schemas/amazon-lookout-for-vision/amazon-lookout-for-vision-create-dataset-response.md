---
description: CreateDatasetResponse schema from Amazon Lookout for Vision API
layout: schema
name: CreateDatasetResponse
properties_list:
- description: ''
  name: DatasetMetadata
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-create-dataset-response-schema.json
slug: amazon-lookout-for-vision-create-dataset-response
source_filename: amazon-lookout-for-vision-create-dataset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-create-dataset-response-schema.json\",\n  \"title\": \"CreateDatasetResponse\",\n  \"description\": \"CreateDatasetResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetMetadata\"\n        },\n        {\n          \"description\": \"Information about the dataset.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-create-dataset-response-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: CreateDatasetResponse
---
