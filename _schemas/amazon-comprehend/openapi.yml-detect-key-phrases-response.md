---
description: DetectKeyPhrasesResponse schema
layout: schema
name: DetectKeyPhrasesResponse
properties_list:
- description: ''
  name: KeyPhrases
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-key-phrases-response-schema.json
slug: openapi.yml-detect-key-phrases-response
source_filename: openapi.yml-detect-key-phrases-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-key-phrases-response-schema.json\",\n  \"title\": \"DetectKeyPhrasesResponse\",\n  \"description\": \"DetectKeyPhrasesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyPhrases\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfKeyPhrases\"\n        },\n        {\n          \"description\": \"A collection of key phrases that Amazon Comprehend identified in the input text. For each key phrase, the response provides the text of the key phrase, where the key phrase begins and ends, and the level of confidence that Amazon Comprehend has in the accuracy of the detection. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-key-phrases-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectKeyPhrasesResponse
---
