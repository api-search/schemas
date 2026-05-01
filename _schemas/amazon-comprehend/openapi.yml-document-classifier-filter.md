---
description: Provides information for filtering a list of document classifiers. You can only specify one filtering parameter in a request. For more information, see the <code>ListDocumentClassifiers</code> operation.
layout: schema
name: DocumentClassifierFilter
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: DocumentClassifierName
  type: object
- description: ''
  name: SubmitTimeBefore
  type: object
- description: ''
  name: SubmitTimeAfter
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-classifier-filter-schema.json
slug: openapi.yml-document-classifier-filter
source_filename: openapi.yml-document-classifier-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-filter-schema.json\",\n  \"title\": \"DocumentClassifierFilter\",\n  \"description\": \"Provides information for filtering a list of document classifiers. You can only specify one filtering parameter in a request. For more information, see the <code>ListDocumentClassifiers</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelStatus\"\n        },\n        {\n          \"description\": \"Filters the list of classifiers based on status.\"\n        }\n      ]\n    },\n    \"DocumentClassifierName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArnName\"\n        },\n        {\n          \"description\": \"The name that you\
  \ assigned to the document classifier\"\n        }\n      ]\n    },\n    \"SubmitTimeBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filters the list of classifiers based on the time that the classifier was submitted for processing. Returns only classifiers submitted before the specified time. Classifiers are returned in ascending order, oldest to newest.\"\n        }\n      ]\n    },\n    \"SubmitTimeAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Filters the list of classifiers based on the time that the classifier was submitted for processing. Returns only classifiers submitted after the specified time. Classifiers are returned in descending order, newest to oldest.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-filter-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentClassifierFilter
---
