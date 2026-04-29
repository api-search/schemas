---
description: Contains metadata describing the lexicon such as the number of lexemes, language code, and so on. For more information, see <a href="https://docs.aws.amazon.com/polly/latest/dg/managing-lexicons.html">Managing Lexicons</a>.
layout: schema
name: LexiconAttributes
properties_list:
- description: ''
  name: Alphabet
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: LastModified
  type: object
- description: ''
  name: LexiconArn
  type: object
- description: ''
  name: LexemesCount
  type: object
- description: ''
  name: Size
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-lexicon-attributes-schema.json
slug: amazon-polly-lexicon-attributes
source_filename: amazon-polly-lexicon-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-lexicon-attributes-schema.json\",\n  \"title\": \"LexiconAttributes\",\n  \"description\": \"Contains metadata describing the lexicon such as the number of lexemes, language code, and so on. For more information, see <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/managing-lexicons.html\\\">Managing Lexicons</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alphabet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alphabet\"\n        },\n        {\n          \"description\": \"Phonetic alphabet used in the lexicon. Valid values are <code>ipa</code> and <code>x-sampa</code>.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n  \
  \        \"description\": \"Language code that the lexicon applies to. A lexicon with a language code such as \\\"en\\\" would be applied to all English languages (en-GB, en-US, en-AUS, en-WLS, and so on.\"\n        }\n      ]\n    },\n    \"LastModified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModified\"\n        },\n        {\n          \"description\": \"Date lexicon was last modified (a timestamp value).\"\n        }\n      ]\n    },\n    \"LexiconArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconArn\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of the lexicon.\"\n        }\n      ]\n    },\n    \"LexemesCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexemesCount\"\n        },\n        {\n          \"description\": \"Number of lexemes in the lexicon.\"\n        }\n      ]\n    },\n    \"Size\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/Size\"\n        },\n        {\n          \"description\": \"Total size of the lexicon, in characters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-lexicon-attributes-schema.json
tags:
- AI
- AWS
- Machine Learning
- Speech Synthesis
- Text-To-Speech
- TTS
- Voice
- SSML
- Neural Engine
- Generative AI
title: LexiconAttributes
---
