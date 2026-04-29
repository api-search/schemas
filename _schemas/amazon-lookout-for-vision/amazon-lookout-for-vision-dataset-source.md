---
description: Information about the location of a manifest file that Amazon Lookout for Vision uses to to create a dataset.
layout: schema
name: DatasetSource
properties_list:
- description: ''
  name: GroundTruthManifest
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-dataset-source-schema.json
slug: amazon-lookout-for-vision-dataset-source
source_filename: amazon-lookout-for-vision-dataset-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-source-schema.json\",\n  \"title\": \"DatasetSource\",\n  \"description\": \"Information about the location of a manifest file that Amazon Lookout for Vision uses to to create a dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroundTruthManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetGroundTruthManifest\"\n        },\n        {\n          \"description\": \"Location information for the manifest file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-source-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DatasetSource
---
