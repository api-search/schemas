---
description: Describes the annotations associated with a entity recognizer.
layout: schema
name: DatasetEntityRecognizerAnnotations
properties_list:
- description: ''
  name: S3Uri
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-dataset-entity-recognizer-annotations-schema.json
slug: openapi.yml-dataset-entity-recognizer-annotations
source_filename: openapi.yml-dataset-entity-recognizer-annotations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-entity-recognizer-annotations-schema.json\",\n  \"title\": \"DatasetEntityRecognizerAnnotations\",\n  \"description\": \"Describes the annotations associated with a entity recognizer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \" Specifies the Amazon S3 location where the training documents for an entity recognizer are located. The URI must be in the same Region as the API endpoint that you are calling.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-entity-recognizer-annotations-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DatasetEntityRecognizerAnnotations
---
