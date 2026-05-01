---
description: The <code>CreatePresetRequest</code> structure.
layout: schema
name: CreatePresetRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Container
  type: object
- description: ''
  name: Video
  type: object
- description: ''
  name: Audio
  type: object
- description: ''
  name: Thumbnails
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-create-preset-request-schema.json
slug: amazon-elastic-transcoder-create-preset-request
source_filename: amazon-elastic-transcoder-create-preset-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-create-preset-request-schema.json\",\n  \"title\": \"CreatePresetRequest\",\n  \"description\": \"The <code>CreatePresetRequest</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the preset. We recommend that the name be unique within the AWS account, but uniqueness is not enforced.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the preset.\"\n        }\n      ]\n    },\n    \"Container\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/PresetContainer\"\n        },\n        {\n          \"description\": \"The container type for the output file. Valid values include <code>flac</code>, <code>flv</code>, <code>fmp4</code>, <code>gif</code>, <code>mp3</code>, <code>mp4</code>, <code>mpg</code>, <code>mxf</code>, <code>oga</code>, <code>ogg</code>, <code>ts</code>, and <code>webm</code>.\"\n        }\n      ]\n    },\n    \"Video\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoParameters\"\n        },\n        {\n          \"description\": \"A section of the request body that specifies the video parameters.\"\n        }\n      ]\n    },\n    \"Audio\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioParameters\"\n        },\n        {\n          \"description\": \"A section of the request body that specifies the audio parameters.\"\n        }\n      ]\n    },\n    \"Thumbnails\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Thumbnails\"\n        },\n        {\n          \"description\": \"A section of the request body that specifies the thumbnail parameters, if any.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Container\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-create-preset-request-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: CreatePresetRequest
---
