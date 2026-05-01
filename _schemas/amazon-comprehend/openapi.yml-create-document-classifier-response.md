---
description: CreateDocumentClassifierResponse schema
layout: schema
name: CreateDocumentClassifierResponse
properties_list:
- description: ''
  name: DocumentClassifierArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-create-document-classifier-response-schema.json
slug: openapi.yml-create-document-classifier-response
source_filename: openapi.yml-create-document-classifier-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-document-classifier-response-schema.json\",\n  \"title\": \"CreateDocumentClassifierResponse\",\n  \"description\": \"CreateDocumentClassifierResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentClassifierArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the document classifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-document-classifier-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: CreateDocumentClassifierResponse
---
