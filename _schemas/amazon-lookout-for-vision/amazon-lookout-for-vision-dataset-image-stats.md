---
description: Statistics about the images in a dataset.
layout: schema
name: DatasetImageStats
properties_list:
- description: ''
  name: Total
  type: object
- description: ''
  name: Labeled
  type: object
- description: ''
  name: Normal
  type: object
- description: ''
  name: Anomaly
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-dataset-image-stats-schema.json
slug: amazon-lookout-for-vision-dataset-image-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-image-stats-schema.json\",\n  \"title\": \"DatasetImageStats\",\n  \"description\": \"Statistics about the images in a dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of images in the dataset.\"\n        }\n      ]\n    },\n    \"Labeled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of labeled images.\"\n        }\n      ]\n    },\n    \"Normal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"\
  description\": \"The total number of images labeled as normal.\"\n        }\n      ]\n    },\n    \"Anomaly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"the total number of images labeled as an anomaly.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-image-stats-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DatasetImageStats
---
