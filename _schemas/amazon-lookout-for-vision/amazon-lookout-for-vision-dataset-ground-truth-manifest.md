---
description: Location information about a manifest file. You can use a manifest file to create a dataset.
layout: schema
name: DatasetGroundTruthManifest
properties_list:
- description: ''
  name: S3Object
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-dataset-ground-truth-manifest-schema.json
slug: amazon-lookout-for-vision-dataset-ground-truth-manifest
source_filename: amazon-lookout-for-vision-dataset-ground-truth-manifest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-ground-truth-manifest-schema.json\",\n  \"title\": \"DatasetGroundTruthManifest\",\n  \"description\": \"Location information about a manifest file. You can use a manifest file to create a dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Object\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputS3Object\"\n        },\n        {\n          \"description\": \"The S3 bucket location for the manifest file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-dataset-ground-truth-manifest-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DatasetGroundTruthManifest
---
