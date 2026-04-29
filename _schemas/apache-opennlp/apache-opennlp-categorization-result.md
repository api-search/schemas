---
description: CategorizationResult schema from Apache OpenNLP
layout: schema
name: CategorizationResult
properties_list:
- description: Most likely category label
  name: bestCategory
  type: string
- description: Probability for each category
  name: probabilities
  type: object
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-categorization-result-schema.json
slug: apache-opennlp-categorization-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-categorization-result-schema.json\",\n  \"title\": \"CategorizationResult\",\n  \"description\": \"CategorizationResult schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bestCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Most likely category label\",\n      \"example\": \"Sports\"\n    },\n    \"probabilities\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"number\"\n      },\n      \"description\": \"Probability for each category\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-categorization-result-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: CategorizationResult
---
