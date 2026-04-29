---
description: DescribeDocumentClassifierResponse schema
layout: schema
name: DescribeDocumentClassifierResponse
properties_list:
- description: ''
  name: DocumentClassifierProperties
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-describe-document-classifier-response-schema.json
slug: openapi.yml-describe-document-classifier-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-document-classifier-response-schema.json\",\n  \"title\": \"DescribeDocumentClassifierResponse\",\n  \"description\": \"DescribeDocumentClassifierResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentClassifierProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierProperties\"\n        },\n        {\n          \"description\": \"An object that contains the properties associated with a document classifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-describe-document-classifier-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DescribeDocumentClassifierResponse
---
