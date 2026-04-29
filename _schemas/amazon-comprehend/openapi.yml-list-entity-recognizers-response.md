---
description: ListEntityRecognizersResponse schema
layout: schema
name: ListEntityRecognizersResponse
properties_list:
- description: ''
  name: EntityRecognizerPropertiesList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-list-entity-recognizers-response-schema.json
slug: openapi.yml-list-entity-recognizers-response
source_filename: openapi.yml-list-entity-recognizers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-entity-recognizers-response-schema.json\",\n  \"title\": \"ListEntityRecognizersResponse\",\n  \"description\": \"ListEntityRecognizersResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntityRecognizerPropertiesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityRecognizerPropertiesList\"\n        },\n        {\n          \"description\": \"The list of properties of an entity recognizer.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifies the next page of results to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-list-entity-recognizers-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ListEntityRecognizersResponse
---
