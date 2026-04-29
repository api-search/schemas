---
description: DescribeVoicesOutput schema from Amazon Polly API
layout: schema
name: DescribeVoicesOutput
properties_list:
- description: ''
  name: Voices
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-describe-voices-output-schema.json
slug: amazon-polly-describe-voices-output
source_filename: amazon-polly-describe-voices-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-describe-voices-output-schema.json\",\n  \"title\": \"DescribeVoicesOutput\",\n  \"description\": \"DescribeVoicesOutput schema from Amazon Polly API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Voices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoiceList\"\n        },\n        {\n          \"description\": \"A list of voices with their properties.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token to use in the next request to continue the listing of voices. <code>NextToken</code> is returned only if the response is truncated.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"\
  Voices\": [\n      {\n        \"Gender\": \"Female\",\n        \"Id\": \"Emma\",\n        \"LanguageCode\": \"en-GB\",\n        \"LanguageName\": \"British English\",\n        \"Name\": \"Emma\"\n      },\n      {\n        \"Gender\": \"Male\",\n        \"Id\": \"Brian\",\n        \"LanguageCode\": \"en-GB\",\n        \"LanguageName\": \"British English\",\n        \"Name\": \"Brian\"\n      },\n      {\n        \"Gender\": \"Female\",\n        \"Id\": \"Amy\",\n        \"LanguageCode\": \"en-GB\",\n        \"LanguageName\": \"British English\",\n        \"Name\": \"Amy\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-describe-voices-output-schema.json
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
title: DescribeVoicesOutput
---
