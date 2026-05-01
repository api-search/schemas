---
description: GetLexiconOutput schema from Amazon Polly API
layout: schema
name: GetLexiconOutput
properties_list:
- description: ''
  name: Lexicon
  type: object
- description: ''
  name: LexiconAttributes
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-get-lexicon-output-schema.json
slug: amazon-polly-get-lexicon-output
source_filename: amazon-polly-get-lexicon-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-get-lexicon-output-schema.json\",\n  \"title\": \"GetLexiconOutput\",\n  \"description\": \"GetLexiconOutput schema from Amazon Polly API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Lexicon\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Lexicon\"\n        },\n        {\n          \"description\": \"Lexicon object that provides name and the string content of the lexicon. \"\n        }\n      ]\n    },\n    \"LexiconAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconAttributes\"\n        },\n        {\n          \"description\": \"Metadata of the lexicon, including phonetic alphabetic used, language code, lexicon ARN, number of lexemes defined in the lexicon, and size of lexicon in bytes.\"\n        }\n\
  \      ]\n    }\n  },\n  \"example\": {\n    \"Lexicon\": {\n      \"Content\": \"<?xml version=\\\"1.0\\\" encoding=\\\"UTF-8\\\"?>\\r\\n<lexicon version=\\\"1.0\\\" \\r\\n      xmlns=\\\"http://www.w3.org/2005/01/pronunciation-lexicon\\\"\\r\\n      xmlns:xsi=\\\"http://www.w3.org/2001/XMLSchema-instance\\\" \\r\\n      xsi:schemaLocation=\\\"http://www.w3.org/2005/01/pronunciation-lexicon \\r\\n        http://www.w3.org/TR/2007/CR-pronunciation-lexicon-20071212/pls.xsd\\\"\\r\\n      alphabet=\\\"ipa\\\" \\r\\n      xml:lang=\\\"en-US\\\">\\r\\n  <lexeme>\\r\\n    <grapheme>W3C</grapheme>\\r\\n    <alias>World Wide Web Consortium</alias>\\r\\n  </lexeme>\\r\\n</lexicon>\",\n      \"Name\": \"example\"\n    },\n    \"LexiconAttributes\": {\n      \"Alphabet\": \"ipa\",\n      \"LanguageCode\": \"en-US\",\n      \"LastModified\": 1478542980.117,\n      \"LexemesCount\": 1,\n      \"LexiconArn\": \"arn:aws:polly:us-east-1:123456789012:lexicon/example\",\n      \"Size\": 503\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-get-lexicon-output-schema.json
tags:
- AI
- Machine Learning
- Speech Synthesis
- Text-To-Speech
- TTS
- Voice
- SSML
- Neural Engine
- Generative AI
title: GetLexiconOutput
---
