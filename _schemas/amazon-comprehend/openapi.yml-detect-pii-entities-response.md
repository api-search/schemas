---
description: DetectPiiEntitiesResponse schema
layout: schema
name: DetectPiiEntitiesResponse
properties_list:
- description: ''
  name: Entities
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-pii-entities-response-schema.json
slug: openapi.yml-detect-pii-entities-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-pii-entities-response-schema.json\",\n  \"title\": \"DetectPiiEntitiesResponse\",\n  \"description\": \"DetectPiiEntitiesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfPiiEntities\"\n        },\n        {\n          \"description\": \"A collection of PII entities identified in the input text. For each entity, the response provides the entity type, where the entity text begins and ends, and the level of confidence that Amazon Comprehend has in the detection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-pii-entities-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectPiiEntitiesResponse
---
