---
description: DetectAnomaliesResponse schema from Amazon Lookout for Vision API
layout: schema
name: DetectAnomaliesResponse
properties_list:
- description: ''
  name: DetectAnomalyResult
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-detect-anomalies-response-schema.json
slug: amazon-lookout-for-vision-detect-anomalies-response
source_filename: amazon-lookout-for-vision-detect-anomalies-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-detect-anomalies-response-schema.json\",\n  \"title\": \"DetectAnomaliesResponse\",\n  \"description\": \"DetectAnomaliesResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DetectAnomalyResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectAnomalyResult\"\n        },\n        {\n          \"description\": \"The results of the <code>DetectAnomalies</code> operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-detect-anomalies-response-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DetectAnomaliesResponse
---
