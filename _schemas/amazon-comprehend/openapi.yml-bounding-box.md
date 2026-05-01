---
description: <p>The bounding box around the detected page or around an element on a document page. The left (x-coordinate) and top (y-coordinate) are coordinates that represent the top and left sides of the bounding box. Note that the upper-left corner of the image is the origin (0,0). </p> <p>For additional information, see <a href="https://docs.aws.amazon.com/textract/latest/dg/API_BoundingBox.html">BoundingBox</a> in the Amazon Textract API reference.</p>
layout: schema
name: BoundingBox
properties_list:
- description: ''
  name: Height
  type: object
- description: ''
  name: Left
  type: object
- description: ''
  name: Top
  type: object
- description: ''
  name: Width
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-bounding-box-schema.json
slug: openapi.yml-bounding-box
source_filename: openapi.yml-bounding-box-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-bounding-box-schema.json\",\n  \"title\": \"BoundingBox\",\n  \"description\": \"<p>The bounding box around the detected page or around an element on a document page. The left (x-coordinate) and top (y-coordinate) are coordinates that represent the top and left sides of the bounding box. Note that the upper-left corner of the image is the origin (0,0). </p> <p>For additional information, see <a href=\\\"https://docs.aws.amazon.com/textract/latest/dg/API_BoundingBox.html\\\">BoundingBox</a> in the Amazon Textract API reference.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The height of the bounding box as a ratio of the overall document\
  \ page height.\"\n        }\n      ]\n    },\n    \"Left\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The left coordinate of the bounding box as a ratio of overall document page width.\"\n        }\n      ]\n    },\n    \"Top\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The top coordinate of the bounding box as a ratio of overall document page height.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The width of the bounding box as a ratio of the overall document page width.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-bounding-box-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: BoundingBox
---
