---
description: DescribeDatasetResponse schema from Amazon Lookout for Vision API
layout: schema
name: DescribeDatasetResponse
properties_list:
- description: ''
  name: DatasetDescription
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-describe-dataset-response-schema.json
slug: amazon-lookout-for-vision-describe-dataset-response
source_filename: amazon-lookout-for-vision-describe-dataset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-describe-dataset-response-schema.json\",\n  \"title\": \"DescribeDatasetResponse\",\n  \"description\": \"DescribeDatasetResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetDescription\"\n        },\n        {\n          \"description\": \"The description of the requested dataset. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-describe-dataset-response-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DescribeDatasetResponse
---
