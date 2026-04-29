---
description: LanguageDetectionResult schema from Apache OpenNLP
layout: schema
name: LanguageDetectionResult
properties_list:
- description: ISO-639-3 code of most likely language
  name: bestLanguage
  type: string
- description: Confidence score 0-1
  name: confidence
  type: number
- description: All detected languages with probabilities
  name: languages
  type: array
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-language-detection-result-schema.json
slug: apache-opennlp-language-detection-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-language-detection-result-schema.json\",\n  \"title\": \"LanguageDetectionResult\",\n  \"description\": \"LanguageDetectionResult schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bestLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"ISO-639-3 code of most likely language\",\n      \"example\": \"eng\"\n    },\n    \"confidence\": {\n      \"type\": \"number\",\n      \"description\": \"Confidence score 0-1\",\n      \"example\": 0.98\n    },\n    \"languages\": {\n      \"type\": \"array\",\n      \"description\": \"All detected languages with probabilities\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LanguageProbability\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-language-detection-result-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: LanguageDetectionResult
---
