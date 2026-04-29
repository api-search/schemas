---
description: ListLexiconsOutput schema from Amazon Polly API
layout: schema
name: ListLexiconsOutput
properties_list:
- description: ''
  name: Lexicons
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-list-lexicons-output-schema.json
slug: amazon-polly-list-lexicons-output
source_filename: amazon-polly-list-lexicons-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-list-lexicons-output-schema.json\",\n  \"title\": \"ListLexiconsOutput\",\n  \"description\": \"ListLexiconsOutput schema from Amazon Polly API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Lexicons\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconDescriptionList\"\n        },\n        {\n          \"description\": \"A list of lexicon names and attributes.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token to use in the next request to continue the listing of lexicons. <code>NextToken</code> is returned only if the response is truncated.\"\n        }\n      ]\n    }\n  },\n  \"example\"\
  : {\n    \"Lexicons\": [\n      {\n        \"Attributes\": {\n          \"Alphabet\": \"ipa\",\n          \"LanguageCode\": \"en-US\",\n          \"LastModified\": 1478542980.117,\n          \"LexemesCount\": 1,\n          \"LexiconArn\": \"arn:aws:polly:us-east-1:123456789012:lexicon/example\",\n          \"Size\": 503\n        },\n        \"Name\": \"example\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-list-lexicons-output-schema.json
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
title: ListLexiconsOutput
---
