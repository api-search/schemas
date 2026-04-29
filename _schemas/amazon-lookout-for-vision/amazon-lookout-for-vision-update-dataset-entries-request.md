---
description: UpdateDatasetEntriesRequest schema from Amazon Lookout for Vision API
layout: schema
name: UpdateDatasetEntriesRequest
properties_list:
- description: ''
  name: Changes
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-update-dataset-entries-request-schema.json
slug: amazon-lookout-for-vision-update-dataset-entries-request
source_filename: amazon-lookout-for-vision-update-dataset-entries-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-update-dataset-entries-request-schema.json\",\n  \"title\": \"UpdateDatasetEntriesRequest\",\n  \"description\": \"UpdateDatasetEntriesRequest schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Changes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetChanges\"\n        },\n        {\n          \"description\": \"The entries to add to the dataset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Changes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-update-dataset-entries-request-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: UpdateDatasetEntriesRequest
---
