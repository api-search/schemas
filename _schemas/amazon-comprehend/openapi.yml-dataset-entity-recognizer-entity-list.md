---
description: <p>Describes the dataset entity list for an entity recognizer model.</p> <p>For more information on how the input file is formatted, see <a href="https://docs.aws.amazon.com/comprehend/latest/dg/prep-training-data-cer.html">Preparing training data</a> in the Comprehend Developer Guide. </p>
layout: schema
name: DatasetEntityRecognizerEntityList
properties_list:
- description: ''
  name: S3Uri
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-dataset-entity-recognizer-entity-list-schema.json
slug: openapi.yml-dataset-entity-recognizer-entity-list
source_filename: openapi.yml-dataset-entity-recognizer-entity-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-entity-recognizer-entity-list-schema.json\",\n  \"title\": \"DatasetEntityRecognizerEntityList\",\n  \"description\": \"<p>Describes the dataset entity list for an entity recognizer model.</p> <p>For more information on how the input file is formatted, see <a href=\\\"https://docs.aws.amazon.com/comprehend/latest/dg/prep-training-data-cer.html\\\">Preparing training data</a> in the Comprehend Developer Guide. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"Specifies the Amazon S3 location where the entity list is located.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-entity-recognizer-entity-list-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DatasetEntityRecognizerEntityList
---
