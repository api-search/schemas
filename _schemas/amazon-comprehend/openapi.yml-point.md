---
description: <p>The X and Y coordinates of a point on a document page.</p> <p>For additional information, see <a href="https://docs.aws.amazon.com/textract/latest/dg/API_Point.html">Point</a> in the Amazon Textract API reference.</p>
layout: schema
name: Point
properties_list:
- description: ''
  name: X
  type: object
- description: ''
  name: Y
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-point-schema.json
slug: openapi.yml-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-point-schema.json\",\n  \"title\": \"Point\",\n  \"description\": \"<p>The X and Y coordinates of a point on a document page.</p> <p>For additional information, see <a href=\\\"https://docs.aws.amazon.com/textract/latest/dg/API_Point.html\\\">Point</a> in the Amazon Textract API reference.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"X\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The value of the X coordinate for a point on a polygon\"\n        }\n      ]\n    },\n    \"Y\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The value of the Y coordinate for a point on a polygon\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-point-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: Point
---
