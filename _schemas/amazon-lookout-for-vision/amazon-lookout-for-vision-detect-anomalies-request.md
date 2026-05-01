---
description: DetectAnomaliesRequest schema from Amazon Lookout for Vision API
layout: schema
name: DetectAnomaliesRequest
properties_list:
- description: ''
  name: Body
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-detect-anomalies-request-schema.json
slug: amazon-lookout-for-vision-detect-anomalies-request
source_filename: amazon-lookout-for-vision-detect-anomalies-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-detect-anomalies-request-schema.json\",\n  \"title\": \"DetectAnomaliesRequest\",\n  \"description\": \"DetectAnomaliesRequest schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Stream\"\n        },\n        {\n          \"description\": \"The unencrypted image bytes that you want to analyze. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Body\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-detect-anomalies-request-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DetectAnomaliesRequest
---
