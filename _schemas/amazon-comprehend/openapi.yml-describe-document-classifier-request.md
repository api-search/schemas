---
description: DescribeDocumentClassifierRequest schema
layout: schema
name: DescribeDocumentClassifierRequest
properties_list:
- description: ''
  name: DocumentClassifierArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-document-classifier-request-schema.json
slug: openapi.yml-describe-document-classifier-request
source_filename: openapi.yml-describe-document-classifier-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-document-classifier-request-schema.json\",\n  \"title\": \"DescribeDocumentClassifierRequest\",\n  \"description\": \"DescribeDocumentClassifierRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentClassifierArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the document classifier. The <code>CreateDocumentClassifier</code> operation returns this identifier in its response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DocumentClassifierArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-document-classifier-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeDocumentClassifierRequest
---
