---
description: StopTrainingDocumentClassifierRequest schema
layout: schema
name: StopTrainingDocumentClassifierRequest
properties_list:
- description: ''
  name: DocumentClassifierArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-stop-training-document-classifier-request-schema.json
slug: openapi.yml-stop-training-document-classifier-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-stop-training-document-classifier-request-schema.json\",\n  \"title\": \"StopTrainingDocumentClassifierRequest\",\n  \"description\": \"StopTrainingDocumentClassifierRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentClassifierArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the document classifier currently being trained.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DocumentClassifierArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-stop-training-document-classifier-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: StopTrainingDocumentClassifierRequest
---
