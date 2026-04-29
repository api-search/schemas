---
description: SynthesizeSpeechInput schema from Amazon Polly API
layout: schema
name: SynthesizeSpeechInput
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
  name: SampleRate
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
schema_file: json-schema/amazon-polly-synthesize-speech-input-schema.json
slug: amazon-polly-synthesize-speech-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-synthesize-speech-input-schema.json\",\n  \"title\": \"SynthesizeSpeechInput\",\n  \"description\": \"SynthesizeSpeechInput schema from Amazon Polly API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Engine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Engine\"\n        },\n        {\n          \"description\": \"<p>Specifies the engine (<code>standard</code> or <code>neural</code>) for Amazon Polly to use when processing input text for speech synthesis. For information on Amazon Polly voices and which voices are available in standard-only, NTTS-only, and both standard and NTTS formats, see <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/voicelist.html\\\">Available Voices</a>.</p> <p> <b>NTTS-only voices</b> </p> <p>When using NTTS-only voices\
  \ such as Kevin (en-US), this parameter is required and must be set to <code>neural</code>. If the engine is not specified, or is set to <code>standard</code>, this will result in an error. </p> <p>Type: String</p> <p>Valid Values: <code>standard</code> | <code>neural</code> </p> <p>Required: Yes</p> <p> <b>Standard voices</b> </p> <p>For standard voices, this is not required; the engine parameter defaults to <code>standard</code>. If the engine is not specified, or is set to <code>standard</code> and an NTTS-only voice is selected, this will result in an error. </p>\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"<p>Optional language code for the Synthesize Speech request. This is only necessary if using a bilingual voice, such as Aditi, which can be used for either Indian English (en-IN) or Hindi (hi-IN). </p> <p>If a bilingual voice is\
  \ used and no language code is specified, Amazon Polly uses the default language of the bilingual voice. The default language for any voice is the one returned by the <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/API_DescribeVoices.html\\\">DescribeVoices</a> operation for the <code>LanguageCode</code> parameter. For example, if no language code is specified, Aditi will use Indian English rather than Hindi.</p>\"\n        }\n      ]\n    },\n    \"LexiconNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconNameList\"\n        },\n        {\n          \"description\": \"List of one or more pronunciation lexicon names you want the service to apply during synthesis. Lexicons are applied only if the language of the lexicon is the same as the language of the voice. For information about storing lexicons, see <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/API_PutLexicon.html\\\">PutLexicon</a>.\"\n        }\n      ]\n    },\n    \"OutputFormat\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputFormat\"\n        },\n        {\n          \"description\": \"<p> The format in which the returned output will be encoded. For audio stream, this will be mp3, ogg_vorbis, or pcm. For speech marks, this will be json. </p> <p>When pcm is used, the content returned is audio/pcm in a signed 16-bit, 1 channel (mono), little-endian format. </p>\"\n        }\n      ]\n    },\n    \"SampleRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleRate\"\n        },\n        {\n          \"description\": \"<p>The audio frequency specified in Hz.</p> <p>The valid values for mp3 and ogg_vorbis are \\\"8000\\\", \\\"16000\\\", \\\"22050\\\", and \\\"24000\\\". The default value for standard voices is \\\"22050\\\". The default value for neural voices is \\\"24000\\\".</p> <p>Valid values for pcm are \\\"8000\\\" and \\\"16000\\\" The default value is \\\"16000\\\". </p>\"\n        }\n\
  \      ]\n    },\n    \"SpeechMarkTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpeechMarkTypeList\"\n        },\n        {\n          \"description\": \"The type of speech marks returned for the input text.\"\n        }\n      ]\n    },\n    \"Text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Text\"\n        },\n        {\n          \"description\": \" Input text to synthesize. If you specify <code>ssml</code> as the <code>TextType</code>, follow the SSML format for the input text. \"\n        }\n      ]\n    },\n    \"TextType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TextType\"\n        },\n        {\n          \"description\": \" Specifies whether the input text is plain text or SSML. The default value is plain text. For more information, see <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/ssml.html\\\">Using SSML</a>.\"\n        }\n      ]\n    },\n    \"VoiceId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VoiceId\"\n        },\n        {\n          \"description\": \" Voice ID to use for the synthesis. You can get a list of available voice IDs by calling the <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/API_DescribeVoices.html\\\">DescribeVoices</a> operation. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OutputFormat\",\n    \"Text\",\n    \"VoiceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-synthesize-speech-input-schema.json
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
title: SynthesizeSpeechInput
---
