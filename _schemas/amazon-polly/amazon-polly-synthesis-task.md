---
description: SynthesisTask object that provides information about a speech synthesis task.
layout: schema
name: SynthesisTask
properties_list:
- description: ''
  name: Engine
  type: object
- description: ''
  name: TaskId
  type: object
- description: ''
  name: TaskStatus
  type: object
- description: ''
  name: TaskStatusReason
  type: object
- description: ''
  name: OutputUri
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: RequestCharacters
  type: object
- description: ''
  name: SnsTopicArn
  type: object
- description: ''
  name: LexiconNames
  type: object
- description: ''
  name: OutputFormat
  type: object
- description: ''
  name: SampleRate
  type: object
- description: ''
  name: SpeechMarkTypes
  type: object
- description: ''
  name: TextType
  type: object
- description: ''
  name: VoiceId
  type: object
- description: ''
  name: LanguageCode
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-synthesis-task-schema.json
slug: amazon-polly-synthesis-task
source_filename: amazon-polly-synthesis-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-synthesis-task-schema.json\",\n  \"title\": \"SynthesisTask\",\n  \"description\": \"SynthesisTask object that provides information about a speech synthesis task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Engine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Engine\"\n        },\n        {\n          \"description\": \"Specifies the engine (<code>standard</code> or <code>neural</code>) for Amazon Polly to use when processing input text for speech synthesis. Using a voice that is not supported for the engine selected will result in an error.\"\n        }\n      ]\n    },\n    \"TaskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskId\"\n        },\n        {\n          \"description\": \"The Amazon Polly generated\
  \ identifier for a speech synthesis task.\"\n        }\n      ]\n    },\n    \"TaskStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStatus\"\n        },\n        {\n          \"description\": \"Current status of the individual speech synthesis task.\"\n        }\n      ]\n    },\n    \"TaskStatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStatusReason\"\n        },\n        {\n          \"description\": \"Reason for the current status of a specific speech synthesis task, including errors if the task has failed.\"\n        }\n      ]\n    },\n    \"OutputUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputUri\"\n        },\n        {\n          \"description\": \"Pathway for the output speech file.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n\
  \          \"description\": \"Timestamp for the time the synthesis task was started.\"\n        }\n      ]\n    },\n    \"RequestCharacters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestCharacters\"\n        },\n        {\n          \"description\": \"Number of billable characters synthesized.\"\n        }\n      ]\n    },\n    \"SnsTopicArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopicArn\"\n        },\n        {\n          \"description\": \"ARN for the SNS topic optionally used for providing status notification for a speech synthesis task.\"\n        }\n      ]\n    },\n    \"LexiconNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconNameList\"\n        },\n        {\n          \"description\": \"List of one or more pronunciation lexicon names you want the service to apply during synthesis. Lexicons are applied only if the language of the lexicon is the same as\
  \ the language of the voice. \"\n        }\n      ]\n    },\n    \"OutputFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputFormat\"\n        },\n        {\n          \"description\": \"The format in which the returned output will be encoded. For audio stream, this will be mp3, ogg_vorbis, or pcm. For speech marks, this will be json. \"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleRate\"\n        },\n        {\n          \"description\": \"<p>The audio frequency specified in Hz.</p> <p>The valid values for mp3 and ogg_vorbis are \\\"8000\\\", \\\"16000\\\", \\\"22050\\\", and \\\"24000\\\". The default value for standard voices is \\\"22050\\\". The default value for neural voices is \\\"24000\\\".</p> <p>Valid values for pcm are \\\"8000\\\" and \\\"16000\\\" The default value is \\\"16000\\\". </p>\"\n        }\n      ]\n    },\n    \"SpeechMarkTypes\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpeechMarkTypeList\"\n        },\n        {\n          \"description\": \"The type of speech marks returned for the input text.\"\n        }\n      ]\n    },\n    \"TextType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TextType\"\n        },\n        {\n          \"description\": \"Specifies whether the input text is plain text or SSML. The default value is plain text. \"\n        }\n      ]\n    },\n    \"VoiceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoiceId\"\n        },\n        {\n          \"description\": \"Voice ID to use for the synthesis. \"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"<p>Optional language code for a synthesis task. This is only necessary if using a bilingual voice,\
  \ such as Aditi, which can be used for either Indian English (en-IN) or Hindi (hi-IN). </p> <p>If a bilingual voice is used and no language code is specified, Amazon Polly uses the default language of the bilingual voice. The default language for any voice is the one returned by the <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/API_DescribeVoices.html\\\">DescribeVoices</a> operation for the <code>LanguageCode</code> parameter. For example, if no language code is specified, Aditi will use Indian English rather than Hindi.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-synthesis-task-schema.json
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
title: SynthesisTask
---
