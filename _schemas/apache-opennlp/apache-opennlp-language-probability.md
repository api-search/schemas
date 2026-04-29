---
description: LanguageProbability schema from Apache OpenNLP
layout: schema
name: LanguageProbability
properties_list:
- description: ISO-639-3 language code
  name: language
  type: string
- description: Probability score
  name: probability
  type: number
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-language-probability-schema.json
slug: apache-opennlp-language-probability
source_filename: apache-opennlp-language-probability-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-language-probability-schema.json\",\n  \"title\": \"LanguageProbability\",\n  \"description\": \"LanguageProbability schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"ISO-639-3 language code\",\n      \"example\": \"eng\"\n    },\n    \"probability\": {\n      \"type\": \"number\",\n      \"description\": \"Probability score\",\n      \"example\": 0.98\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-language-probability-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: LanguageProbability
---
