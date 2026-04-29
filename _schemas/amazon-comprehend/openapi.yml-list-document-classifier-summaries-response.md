---
description: ListDocumentClassifierSummariesResponse schema
layout: schema
name: ListDocumentClassifierSummariesResponse
properties_list:
- description: ''
  name: DocumentClassifierSummariesList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-document-classifier-summaries-response-schema.json
slug: openapi.yml-list-document-classifier-summaries-response
source_filename: openapi.yml-list-document-classifier-summaries-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-document-classifier-summaries-response-schema.json\",\n  \"title\": \"ListDocumentClassifierSummariesResponse\",\n  \"description\": \"ListDocumentClassifierSummariesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentClassifierSummariesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierSummariesList\"\n        },\n        {\n          \"description\": \"The list of summaries of document classifiers.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifies the next page of results to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-document-classifier-summaries-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListDocumentClassifierSummariesResponse
---
