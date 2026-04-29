---
description: ContainsPiiEntitiesResponse schema
layout: schema
name: ContainsPiiEntitiesResponse
properties_list:
- description: ''
  name: Labels
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-contains-pii-entities-response-schema.json
slug: openapi.yml-contains-pii-entities-response
source_filename: openapi.yml-contains-pii-entities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-contains-pii-entities-response-schema.json\",\n  \"title\": \"ContainsPiiEntitiesResponse\",\n  \"description\": \"ContainsPiiEntitiesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Labels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfEntityLabels\"\n        },\n        {\n          \"description\": \"The labels used in the document being analyzed. Individual labels represent personally identifiable information (PII) entity types.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-contains-pii-entities-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ContainsPiiEntitiesResponse
---
