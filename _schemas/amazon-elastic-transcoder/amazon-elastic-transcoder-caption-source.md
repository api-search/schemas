---
description: A source file for the input sidecar captions used during the transcoding process.
layout: schema
name: CaptionSource
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Language
  type: object
- description: ''
  name: TimeOffset
  type: object
- description: ''
  name: Label
  type: object
- description: ''
  name: Encryption
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-caption-source-schema.json
slug: amazon-elastic-transcoder-caption-source
source_filename: amazon-elastic-transcoder-caption-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-caption-source-schema.json\",\n  \"title\": \"CaptionSource\",\n  \"description\": \"A source file for the input sidecar captions used during the transcoding process.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongKey\"\n        },\n        {\n          \"description\": \"The name of the sidecar caption file that you want Elastic Transcoder to include in the output file.\"\n        }\n      ]\n    },\n    \"Language\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \"<p>A string that specifies the language of the caption. If you specified multiple inputs with captions, the caption language\
  \ must match in order to be included in the output. Specify this as one of:</p> <ul> <li> <p>2-character ISO 639-1 code</p> </li> <li> <p>3-character ISO 639-2 code</p> </li> </ul> <p>For more information on ISO language codes and language names, see the List of ISO 639-1 codes.</p>\"\n        }\n      ]\n    },\n    \"TimeOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeOffset\"\n        },\n        {\n          \"description\": \"<p>For clip generation or captions that do not start at the same time as the associated video file, the <code>TimeOffset</code> tells Elastic Transcoder how much of the video to encode before including captions.</p> <p>Specify the TimeOffset in the form [+-]SS.sss or [+-]HH:mm:SS.ss.</p>\"\n        }\n      ]\n    },\n    \"Label\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The label of the caption shown in the player when\
  \ choosing a language. We recommend that you put the caption language name here, in the language of the captions.\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"description\": \"The encryption settings, if any, that Elastic Transcoder needs to decyrpt your caption sources, or that you want Elastic Transcoder to apply to your caption sources.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-caption-source-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: CaptionSource
---
