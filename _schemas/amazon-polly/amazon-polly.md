---
description: Schema defining the structure of Amazon Polly speech synthesis resources, including voice configurations, lexicons, and synthesis task parameters for converting text to lifelike speech.
layout: schema
name: Amazon Polly Speech Synthesis Definition
properties_list:
- description: Specifies the engine for Amazon Polly to use when processing input text.
  name: Engine
  type: string
- description: The language identification tag for the voice.
  name: LanguageCode
  type: string
- description: List of one or more pronunciation lexicon names to apply during synthesis.
  name: LexiconNames
  type: array
- description: The format in which the returned output will be encoded.
  name: OutputFormat
  type: string
- description: The audio frequency specified in Hz.
  name: SampleRate
  type: string
- description: The type of speech marks returned for the input text.
  name: SpeechMarkTypes
  type: array
- description: The input text to synthesize.
  name: Text
  type: string
- description: Specifies whether the input text is plain text or SSML.
  name: TextType
  type: string
- description: The voice ID to use for the synthesis.
  name: VoiceId
  type: string
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-schema.json
slug: amazon-polly
source_filename: amazon-polly-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-polly/speech-synthesis-definition\",\n  \"title\": \"Amazon Polly Speech Synthesis Definition\",\n  \"description\": \"Schema defining the structure of Amazon Polly speech synthesis resources, including voice configurations, lexicons, and synthesis task parameters for converting text to lifelike speech.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"OutputFormat\",\n    \"Text\",\n    \"VoiceId\"\n  ],\n  \"properties\": {\n    \"Engine\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"standard\",\n        \"neural\",\n        \"long-form\",\n        \"generative\"\n      ],\n      \"description\": \"Specifies the engine for Amazon Polly to use when processing input text.\"\n    },\n    \"LanguageCode\": {\n      \"type\": \"string\",\n      \"description\": \"The language identification tag for the voice.\"\n    },\n    \"LexiconNames\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[0-9A-Za-z]{1,20}$\"\n      },\n      \"maxItems\": 5,\n      \"description\": \"List of one or more pronunciation lexicon names to apply during synthesis.\"\n    },\n    \"OutputFormat\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"json\",\n        \"mp3\",\n        \"ogg_vorbis\",\n        \"pcm\"\n      ],\n      \"description\": \"The format in which the returned output will be encoded.\"\n    },\n    \"SampleRate\": {\n      \"type\": \"string\",\n      \"description\": \"The audio frequency specified in Hz.\",\n      \"enum\": [\n        \"8000\",\n        \"16000\",\n        \"22050\",\n        \"24000\"\n      ]\n    },\n    \"SpeechMarkTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"sentence\",\n          \"ssml\",\n          \"viseme\",\n          \"word\"\n        ]\n      },\n\
  \      \"description\": \"The type of speech marks returned for the input text.\"\n    },\n    \"Text\": {\n      \"type\": \"string\",\n      \"description\": \"The input text to synthesize.\",\n      \"maxLength\": 3000\n    },\n    \"TextType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ssml\",\n        \"text\"\n      ],\n      \"description\": \"Specifies whether the input text is plain text or SSML.\"\n    },\n    \"VoiceId\": {\n      \"type\": \"string\",\n      \"description\": \"The voice ID to use for the synthesis.\"\n    }\n  },\n  \"$defs\": {\n    \"Voice\": {\n      \"type\": \"object\",\n      \"description\": \"Description of an Amazon Polly voice.\",\n      \"properties\": {\n        \"Gender\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Female\",\n            \"Male\"\n          ],\n          \"description\": \"Gender of the voice.\"\n        },\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Amazon Polly assigned voice ID.\"\n        },\n        \"LanguageCode\": {\n          \"type\": \"string\",\n          \"description\": \"Language code of the voice.\"\n        },\n        \"LanguageName\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name of the language.\"\n        },\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the voice.\"\n        },\n        \"AdditionalLanguageCodes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Additional language codes the voice supports.\"\n        },\n        \"SupportedEngines\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"standard\",\n              \"neural\",\n              \"long-form\",\n              \"generative\"\n            ]\n          },\n          \"description\":\
  \ \"Specifies which engines are supported by the voice.\"\n        }\n      }\n    },\n    \"Lexicon\": {\n      \"type\": \"object\",\n      \"description\": \"A pronunciation lexicon stored in an AWS Region.\",\n      \"properties\": {\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the lexicon.\",\n          \"pattern\": \"^[0-9A-Za-z]{1,20}$\"\n        },\n        \"Content\": {\n          \"type\": \"string\",\n          \"description\": \"Lexicon content in PLS format.\"\n        },\n        \"LexiconArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the lexicon.\"\n        },\n        \"LexemesCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of lexemes in the lexicon.\"\n        },\n        \"Size\": {\n          \"type\": \"integer\",\n          \"description\": \"Total size of the lexicon in characters.\"\n        },\n        \"Alphabet\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Phonetic alphabet used in the lexicon.\",\n          \"enum\": [\n            \"ipa\",\n            \"x-sampa\"\n          ]\n        },\n        \"LanguageCode\": {\n          \"type\": \"string\",\n          \"description\": \"Language code the lexicon applies to.\"\n        },\n        \"LastModified\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the lexicon was last modified.\"\n        }\n      }\n    },\n    \"SynthesisTask\": {\n      \"type\": \"object\",\n      \"description\": \"An asynchronous speech synthesis task.\",\n      \"properties\": {\n        \"TaskId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the synthesis task.\"\n        },\n        \"TaskStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"scheduled\",\n            \"inProgress\",\n            \"completed\",\n            \"failed\"\
  \n          ],\n          \"description\": \"Current status of the synthesis task.\"\n        },\n        \"TaskStatusReason\": {\n          \"type\": \"string\",\n          \"description\": \"Reason for the current status of the task.\"\n        },\n        \"OutputUri\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Pathway for the output speech file.\"\n        },\n        \"OutputFormat\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"json\",\n            \"mp3\",\n            \"ogg_vorbis\",\n            \"pcm\"\n          ]\n        },\n        \"Engine\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"standard\",\n            \"neural\",\n            \"long-form\",\n            \"generative\"\n          ]\n        },\n        \"VoiceId\": {\n          \"type\": \"string\"\n        },\n        \"LanguageCode\": {\n          \"type\": \"string\"\n        },\n        \"CreationTime\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"RequestCharacters\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of billable characters in the request.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-schema.json
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
title: Amazon Polly Speech Synthesis Definition
---
