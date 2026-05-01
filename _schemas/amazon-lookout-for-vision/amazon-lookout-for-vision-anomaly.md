---
description: Information about an anomaly type found on an image by an image segmentation model. For more information, see <a>DetectAnomalies</a>.
layout: schema
name: Anomaly
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: PixelAnomaly
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-anomaly-schema.json
slug: amazon-lookout-for-vision-anomaly
source_filename: amazon-lookout-for-vision-anomaly-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-anomaly-schema.json\",\n  \"title\": \"Anomaly\",\n  \"description\": \"Information about an anomaly type found on an image by an image segmentation model. For more information, see <a>DetectAnomalies</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyName\"\n        },\n        {\n          \"description\": \"The name of an anomaly type found in an image. <code>Name</code> maps to an anomaly type in the training dataset, apart from the anomaly type <code>background</code>. The service automatically inserts the <code>background</code> anomaly type into the response from <code>DetectAnomalies</code>. \"\n        }\n      ]\n    },\n    \"PixelAnomaly\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/PixelAnomaly\"\n        },\n        {\n          \"description\": \"Information about the pixel mask that covers an anomaly type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-anomaly-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: Anomaly
---
