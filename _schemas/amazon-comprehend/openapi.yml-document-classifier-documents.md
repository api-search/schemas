---
description: The location of the training documents. This parameter is required in a request to create a native classifier model.
layout: schema
name: DocumentClassifierDocuments
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: TestS3Uri
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-classifier-documents-schema.json
slug: openapi.yml-document-classifier-documents
source_filename: openapi.yml-document-classifier-documents-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-documents-schema.json\",\n  \"title\": \"DocumentClassifierDocuments\",\n  \"description\": \"The location of the training documents. This parameter is required in a request to create a native classifier model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The S3 URI location of the training documents specified in the S3Uri CSV file.\"\n        }\n      ]\n    },\n    \"TestS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The S3 URI location of the test documents included in the TestS3Uri CSV file. This field is not required\
  \ if you do not specify a test CSV file.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-documents-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentClassifierDocuments
---
