---
description: ListEntityRecognizerSummariesResponse schema
layout: schema
name: ListEntityRecognizerSummariesResponse
properties_list:
- description: ''
  name: EntityRecognizerSummariesList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-entity-recognizer-summaries-response-schema.json
slug: openapi.yml-list-entity-recognizer-summaries-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-entity-recognizer-summaries-response-schema.json\",\n  \"title\": \"ListEntityRecognizerSummariesResponse\",\n  \"description\": \"ListEntityRecognizerSummariesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntityRecognizerSummariesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerSummariesList\"\n        },\n        {\n          \"description\": \"The list entity recognizer summaries.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifies the next page of results to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-entity-recognizer-summaries-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListEntityRecognizerSummariesResponse
---
