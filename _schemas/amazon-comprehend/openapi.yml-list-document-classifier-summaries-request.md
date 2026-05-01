---
description: ListDocumentClassifierSummariesRequest schema
layout: schema
name: ListDocumentClassifierSummariesRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-document-classifier-summaries-request-schema.json
slug: openapi.yml-list-document-classifier-summaries-request
source_filename: openapi.yml-list-document-classifier-summaries-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-document-classifier-summaries-request-schema.json\",\n  \"title\": \"ListDocumentClassifierSummariesRequest\",\n  \"description\": \"ListDocumentClassifierSummariesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifies the next page of results to return.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResultsInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return on each page. The default is 100.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-document-classifier-summaries-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListDocumentClassifierSummariesRequest
---
