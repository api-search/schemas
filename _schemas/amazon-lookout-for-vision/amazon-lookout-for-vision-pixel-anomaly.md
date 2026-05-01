---
description: Information about the pixels in an anomaly mask. For more information, see <a>Anomaly</a>. <code>PixelAnomaly</code> is only returned by image segmentation models.
layout: schema
name: PixelAnomaly
properties_list:
- description: ''
  name: TotalPercentageArea
  type: object
- description: ''
  name: Color
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-pixel-anomaly-schema.json
slug: amazon-lookout-for-vision-pixel-anomaly
source_filename: amazon-lookout-for-vision-pixel-anomaly-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-pixel-anomaly-schema.json\",\n  \"title\": \"PixelAnomaly\",\n  \"description\": \"Information about the pixels in an anomaly mask. For more information, see <a>Anomaly</a>. <code>PixelAnomaly</code> is only returned by image segmentation models.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TotalPercentageArea\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The percentage area of the image that the anomaly type covers.\"\n        }\n      ]\n    },\n    \"Color\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Color\"\n        },\n        {\n          \"description\": \"A hex color value for the mask that covers an anomaly type. Each anomaly\
  \ type has a different mask color. The color maps to the color of the anomaly type used in the training dataset. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-pixel-anomaly-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: PixelAnomaly
---
