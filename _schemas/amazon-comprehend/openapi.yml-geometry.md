---
description: <p>Information about the location of items on a document page.</p> <p>For additional information, see <a href="https://docs.aws.amazon.com/textract/latest/dg/API_Geometry.html">Geometry</a> in the Amazon Textract API reference.</p>
layout: schema
name: Geometry
properties_list:
- description: ''
  name: BoundingBox
  type: object
- description: ''
  name: Polygon
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-geometry-schema.json
slug: openapi.yml-geometry
source_filename: openapi.yml-geometry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-geometry-schema.json\",\n  \"title\": \"Geometry\",\n  \"description\": \"<p>Information about the location of items on a document page.</p> <p>For additional information, see <a href=\\\"https://docs.aws.amazon.com/textract/latest/dg/API_Geometry.html\\\">Geometry</a> in the Amazon Textract API reference.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BoundingBox\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoundingBox\"\n        },\n        {\n          \"description\": \"An axis-aligned coarse representation of the location of the recognized item on the document page.\"\n        }\n      ]\n    },\n    \"Polygon\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Polygon\"\n        },\n        {\n          \"description\"\
  : \"Within the bounding box, a fine-grained polygon around the recognized item.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-geometry-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: Geometry
---
