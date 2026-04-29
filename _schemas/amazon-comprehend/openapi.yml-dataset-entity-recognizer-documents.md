---
description: Describes the documents submitted with a dataset for an entity recognizer model.
layout: schema
name: DatasetEntityRecognizerDocuments
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: InputFormat
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-dataset-entity-recognizer-documents-schema.json
slug: openapi.yml-dataset-entity-recognizer-documents
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-entity-recognizer-documents-schema.json\",\n  \"title\": \"DatasetEntityRecognizerDocuments\",\n  \"description\": \"Describes the documents submitted with a dataset for an entity recognizer model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \" Specifies the Amazon S3 location where the documents for the dataset are located. \"\n        }\n      ]\n    },\n    \"InputFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputFormat\"\n        },\n        {\n          \"description\": \" Specifies how the text in an input file should be processed. This is optional, and the default is ONE_DOC_PER_LINE.\
  \ ONE_DOC_PER_FILE - Each file is considered a separate document. Use this option when you are processing large documents, such as newspaper articles or scientific papers. ONE_DOC_PER_LINE - Each line in a file is considered a separate document. Use this option when you are processing many short documents, such as text messages.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dataset-entity-recognizer-documents-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DatasetEntityRecognizerDocuments
---
