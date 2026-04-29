---
description: DetectDominantLanguageResponse schema
layout: schema
name: DetectDominantLanguageResponse
properties_list:
- description: ''
  name: Languages
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-detect-dominant-language-response-schema.json
slug: openapi.yml-detect-dominant-language-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-dominant-language-response-schema.json\",\n  \"title\": \"DetectDominantLanguageResponse\",\n  \"description\": \"DetectDominantLanguageResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Languages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfDominantLanguages\"\n        },\n        {\n          \"description\": \"<p>Array of languages that Amazon Comprehend detected in the input text. The array is sorted in descending order of the score (the dominant language is always the first element in the array).</p> <p>For each language, the response returns the RFC 5646 language code and the level of confidence that Amazon Comprehend has in the accuracy of its inference. For more information about RFC 5646, see <a href=\\\"https://tools.ietf.org/html/rfc5646\\\
  \">Tags for Identifying Languages</a> on the <i>IETF Tools</i> web site.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-detect-dominant-language-response-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DetectDominantLanguageResponse
---
