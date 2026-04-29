---
description: Response from the DetectLabels operation.
layout: schema
name: DetectLabelsResponse
properties_list:
- description: An array of labels for the real-world objects detected.
  name: Labels
  type: array
- description: The value of OrientationCorrection is always null.
  name: OrientationCorrection
  type: string
- description: Version number of the label detection model used.
  name: LabelModelVersion
  type: string
- description: Information about the quality and dominant colors of an input image.
  name: ImageProperties
  type: object
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detect-labels-response-schema.json
slug: amazon-rekognition-detect-labels-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-labels-response-schema.json\",\n  \"title\": \"DetectLabelsResponse\",\n  \"description\": \"Response from the DetectLabels operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Labels\": {\n      \"type\": \"array\",\n      \"description\": \"An array of labels for the real-world objects detected.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Label\"\n      }\n    },\n    \"OrientationCorrection\": {\n      \"type\": \"string\",\n      \"description\": \"The value of OrientationCorrection is always null.\",\n      \"example\": \"ROTATE_0\"\n    },\n    \"LabelModelVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version number of the label detection model used.\",\n      \"example\": \"3.0\"\n    },\n    \"ImageProperties\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Information about the quality and dominant colors of an input image.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detect-labels-response-schema.json
tags:
- AWS
- Celebrity Recognition
- Computer Vision
- Content Moderation
- Custom Labels
- Deep Learning
- Face Liveness
- Facial Recognition
- Image Analysis
- Machine Learning
- Object Detection
- Text Detection
- Video Analysis
title: DetectLabelsResponse
---
