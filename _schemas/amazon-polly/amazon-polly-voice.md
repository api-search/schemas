---
description: Description of the voice.
layout: schema
name: Voice
properties_list:
- description: ''
  name: Gender
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: LanguageName
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: AdditionalLanguageCodes
  type: object
- description: ''
  name: SupportedEngines
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-voice-schema.json
slug: amazon-polly-voice
source_filename: amazon-polly-voice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-voice-schema.json\",\n  \"title\": \"Voice\",\n  \"description\": \"Description of the voice.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Gender\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Gender\"\n        },\n        {\n          \"description\": \"Gender of the voice.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoiceId\"\n        },\n        {\n          \"description\": \"Amazon Polly assigned voice ID. This is the ID that you specify when calling the <code>SynthesizeSpeech</code> operation.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n        \
  \  \"description\": \"Language code of the voice.\"\n        }\n      ]\n    },\n    \"LanguageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageName\"\n        },\n        {\n          \"description\": \"Human readable name of the language in English.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoiceName\"\n        },\n        {\n          \"description\": \"Name of the voice (for example, Salli, Kendra, etc.). This provides a human readable voice name that you might display in your application.\"\n        }\n      ]\n    },\n    \"AdditionalLanguageCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCodeList\"\n        },\n        {\n          \"description\": \"<p>Additional codes for languages available for the specified voice in addition to its default language. </p> <p>For example, the default language for Aditi is Indian\
  \ English (en-IN) because it was first used for that language. Since Aditi is bilingual and fluent in both Indian English and Hindi, this parameter would show the code <code>hi-IN</code>.</p>\"\n        }\n      ]\n    },\n    \"SupportedEngines\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineList\"\n        },\n        {\n          \"description\": \"Specifies which engines (<code>standard</code> or <code>neural</code>) that are supported by a given voice.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-voice-schema.json
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
title: Voice
---
