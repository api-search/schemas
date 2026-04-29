---
description: Specifies one of the label or labels that categorize the personally identifiable information (PII) entity being analyzed.
layout: schema
name: EntityLabel
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Score
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-entity-label-schema.json
slug: openapi.yml-entity-label
source_filename: openapi.yml-entity-label-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-label-schema.json\",\n  \"title\": \"EntityLabel\",\n  \"description\": \"Specifies one of the label or labels that categorize the personally identifiable information (PII) entity being analyzed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PiiEntityType\"\n        },\n        {\n          \"description\": \"The name of the label.\"\n        }\n      ]\n    },\n    \"Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The level of confidence that Amazon Comprehend has in the accuracy of the detection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-entity-label-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: EntityLabel
---
