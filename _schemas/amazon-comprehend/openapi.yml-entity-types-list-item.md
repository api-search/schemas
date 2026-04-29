---
description: An entity type within a labeled training dataset that Amazon Comprehend uses to train a custom entity recognizer.
layout: schema
name: EntityTypesListItem
properties_list:
- description: ''
  name: Type
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-types-list-item-schema.json
slug: openapi.yml-entity-types-list-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-types-list-item-schema.json\",\n  \"title\": \"EntityTypesListItem\",\n  \"description\": \"An entity type within a labeled training dataset that Amazon Comprehend uses to train a custom entity recognizer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityTypeName\"\n        },\n        {\n          \"description\": \"<p>An entity type within a labeled training dataset that Amazon Comprehend uses to train a custom entity recognizer.</p> <p>Entity types must not contain the following invalid characters: \\\\n (line break), \\\\\\\\n (escaped line break, \\\\r (carriage return), \\\\\\\\r (escaped carriage return), \\\\t (tab), \\\\\\\\t (escaped tab), space, and , (comma).</p>\"\n      \
  \  }\n      ]\n    }\n  },\n  \"required\": [\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-types-list-item-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityTypesListItem
---
