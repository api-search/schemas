---
description: StartSpeechSynthesisTaskInput schema from Amazon Polly API
layout: schema
name: StartSpeechSynthesisTaskInput
properties_list:
- description: ''
  name: Engine
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: LexiconNames
  type: object
- description: ''
  name: OutputFormat
  type: object
- description: ''
  name: OutputS3BucketName
  type: object
- description: ''
  name: OutputS3KeyPrefix
  type: object
- description: ''
  name: SampleRate
  type: object
- description: ''
  name: SnsTopicArn
  type: object
- description: ''
  name: SpeechMarkTypes
  type: object
- description: ''
  name: Text
  type: object
- description: ''
  name: TextType
  type: object
- description: ''
  name: VoiceId
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-start-speech-synthesis-task-input-schema.json
slug: amazon-polly-start-speech-synthesis-task-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-start-speech-synthesis-task-input-schema.json\",\n  \"title\": \"StartSpeechSynthesisTaskInput\",\n  \"description\": \"StartSpeechSynthesisTaskInput schema from Amazon Polly API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Engine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Engine\"\n        },\n        {\n          \"description\": \"Specifies the engine (<code>standard</code> or <code>neural</code>) for Amazon Polly to use when processing input text for speech synthesis. Using a voice that is not supported for the engine selected will result in an error.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\"\
  : \"<p>Optional language code for the Speech Synthesis request. This is only necessary if using a bilingual voice, such as Aditi, which can be used for either Indian English (en-IN) or Hindi (hi-IN). </p> <p>If a bilingual voice is used and no language code is specified, Amazon Polly uses the default language of the bilingual voice. The default language for any voice is the one returned by the <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/API_DescribeVoices.html\\\">DescribeVoices</a> operation for the <code>LanguageCode</code> parameter. For example, if no language code is specified, Aditi will use Indian English rather than Hindi.</p>\"\n        }\n      ]\n    },\n    \"LexiconNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconNameList\"\n        },\n        {\n          \"description\": \"List of one or more pronunciation lexicon names you want the service to apply during synthesis. Lexicons are applied only if the language of the\
  \ lexicon is the same as the language of the voice. \"\n        }\n      ]\n    },\n    \"OutputFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputFormat\"\n        },\n        {\n          \"description\": \"The format in which the returned output will be encoded. For audio stream, this will be mp3, ogg_vorbis, or pcm. For speech marks, this will be json. \"\n        }\n      ]\n    },\n    \"OutputS3BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputS3BucketName\"\n        },\n        {\n          \"description\": \"Amazon S3 bucket name to which the output file will be saved.\"\n        }\n      ]\n    },\n    \"OutputS3KeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputS3KeyPrefix\"\n        },\n        {\n          \"description\": \"The Amazon S3 key prefix for the output speech file.\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/SampleRate\"\n        },\n        {\n          \"description\": \"<p>The audio frequency specified in Hz.</p> <p>The valid values for mp3 and ogg_vorbis are \\\"8000\\\", \\\"16000\\\", \\\"22050\\\", and \\\"24000\\\". The default value for standard voices is \\\"22050\\\". The default value for neural voices is \\\"24000\\\".</p> <p>Valid values for pcm are \\\"8000\\\" and \\\"16000\\\" The default value is \\\"16000\\\". </p>\"\n        }\n      ]\n    },\n    \"SnsTopicArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopicArn\"\n        },\n        {\n          \"description\": \"ARN for the SNS topic optionally used for providing status notification for a speech synthesis task.\"\n        }\n      ]\n    },\n    \"SpeechMarkTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpeechMarkTypeList\"\n        },\n        {\n          \"description\": \"The\
  \ type of speech marks returned for the input text.\"\n        }\n      ]\n    },\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Text\"\n        },\n        {\n          \"description\": \"The input text to synthesize. If you specify ssml as the TextType, follow the SSML format for the input text. \"\n        }\n      ]\n    },\n    \"TextType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TextType\"\n        },\n        {\n          \"description\": \"Specifies whether the input text is plain text or SSML. The default value is plain text. \"\n        }\n      ]\n    },\n    \"VoiceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoiceId\"\n        },\n        {\n          \"description\": \"Voice ID to use for the synthesis. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OutputFormat\",\n    \"OutputS3BucketName\",\n    \"Text\",\n    \"VoiceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-start-speech-synthesis-task-input-schema.json
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
title: StartSpeechSynthesisTaskInput
---
