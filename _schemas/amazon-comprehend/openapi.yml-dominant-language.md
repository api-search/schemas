---
description: Returns the code for the dominant language in the input text and the level of confidence that Amazon Comprehend has in the accuracy of the detection.
layout: schema
name: DominantLanguage
properties_list:
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: Score
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-dominant-language-schema.json
slug: openapi.yml-dominant-language
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dominant-language-schema.json\",\n  \"title\": \"DominantLanguage\",\n  \"description\": \"Returns the code for the dominant language in the input text and the level of confidence that Amazon Comprehend has in the accuracy of the detection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The RFC 5646 language code for the dominant language. For more information about RFC 5646, see <a href=\\\"https://tools.ietf.org/html/rfc5646\\\">Tags for Identifying Languages</a> on the <i>IETF Tools</i> web site.\"\n        }\n      ]\n    },\n    \"Score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\
  \n        },\n        {\n          \"description\": \"The level of confidence that Amazon Comprehend has in the accuracy of the detection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-dominant-language-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DominantLanguage
---
