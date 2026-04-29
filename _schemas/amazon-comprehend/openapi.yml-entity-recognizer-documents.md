---
description: Describes the training documents submitted with an entity recognizer.
layout: schema
name: EntityRecognizerDocuments
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: TestS3Uri
  type: object
- description: ''
  name: InputFormat
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-recognizer-documents-schema.json
slug: openapi.yml-entity-recognizer-documents
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-documents-schema.json\",\n  \"title\": \"EntityRecognizerDocuments\",\n  \"description\": \"Describes the training documents submitted with an entity recognizer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \" Specifies the Amazon S3 location where the training documents for an entity recognizer are located. The URI must be in the same Region as the API endpoint that you are calling.\"\n        }\n      ]\n    },\n    \"TestS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \" Specifies the Amazon S3 location where the test documents\
  \ for an entity recognizer are located. The URI must be in the same Amazon Web Services Region as the API endpoint that you are calling.\"\n        }\n      ]\n    },\n    \"InputFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputFormat\"\n        },\n        {\n          \"description\": \" Specifies how the text in an input file should be processed. This is optional, and the default is ONE_DOC_PER_LINE. ONE_DOC_PER_FILE - Each file is considered a separate document. Use this option when you are processing large documents, such as newspaper articles or scientific papers. ONE_DOC_PER_LINE - Each line in a file is considered a separate document. Use this option when you are processing many short documents, such as text messages.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-recognizer-documents-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityRecognizerDocuments
---
