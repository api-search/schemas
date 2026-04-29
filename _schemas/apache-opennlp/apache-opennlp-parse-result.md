---
description: ParseResult schema from Apache OpenNLP
layout: schema
name: ParseResult
properties_list:
- description: Penn Treebank-style parse tree
  name: parseTree
  type: string
- description: Parse probability
  name: probability
  type: number
provider_name: Apache OpenNLP
provider_slug: apache-opennlp
schema_file: json-schema/apache-opennlp-parse-result-schema.json
slug: apache-opennlp-parse-result
source_filename: apache-opennlp-parse-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-parse-result-schema.json\",\n  \"title\": \"ParseResult\",\n  \"description\": \"ParseResult schema from Apache OpenNLP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parseTree\": {\n      \"type\": \"string\",\n      \"description\": \"Penn Treebank-style parse tree\",\n      \"example\": \"(S (NP Pierre Vinken) (VP will join (NP the board)))\"\n    },\n    \"probability\": {\n      \"type\": \"number\",\n      \"description\": \"Parse probability\",\n      \"example\": 0.87\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-opennlp/refs/heads/main/json-schema/apache-opennlp-parse-result-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Processing
- Apache
- Open Source
- Java
title: ParseResult
---
