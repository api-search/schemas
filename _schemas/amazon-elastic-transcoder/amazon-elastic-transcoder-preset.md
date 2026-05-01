---
description: Presets are templates that contain most of the settings for transcoding media files from one format to another. Elastic Transcoder includes some default presets for common formats, for example, several iPod and iPhone versions. You can also create your own presets for formats that aren't included among the default presets. You specify which preset you want to use when you create a job.
layout: schema
name: Preset
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Arn
  type: object
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
  name: Audio
  type: object
- description: ''
  name: Video
  type: object
- description: ''
  name: Thumbnails
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-preset-schema.json
slug: amazon-elastic-transcoder-preset
source_filename: amazon-elastic-transcoder-preset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-preset-schema.json\",\n  \"title\": \"Preset\",\n  \"description\": \"Presets are templates that contain most of the settings for transcoding media files from one format to another. Elastic Transcoder includes some default presets for common formats, for example, several iPod and iPhone versions. You can also create your own presets for formats that aren't included among the default presets. You specify which preset you want to use when you create a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"Identifier for the new preset. You use this value to get settings for the preset or to delete it.\"\n        }\n      ]\n\
  \    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the preset.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the preset.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the preset.\"\n        }\n      ]\n    },\n    \"Container\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PresetContainer\"\n        },\n        {\n          \"description\": \"The container type for the output file. Valid values include <code>flac</code>, <code>flv</code>, <code>fmp4</code>, <code>gif</code>, <code>mp3</code>, <code>mp4</code>,\
  \ <code>mpg</code>, <code>mxf</code>, <code>oga</code>, <code>ogg</code>, <code>ts</code>, and <code>webm</code>.\"\n        }\n      ]\n    },\n    \"Audio\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioParameters\"\n        },\n        {\n          \"description\": \"A section of the response body that provides information about the audio preset values.\"\n        }\n      ]\n    },\n    \"Video\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoParameters\"\n        },\n        {\n          \"description\": \"A section of the response body that provides information about the video preset values.\"\n        }\n      ]\n    },\n    \"Thumbnails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Thumbnails\"\n        },\n        {\n          \"description\": \"A section of the response body that provides information about the thumbnail preset values, if any.\"\n        }\n      ]\n    },\n\
  \    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PresetType\"\n        },\n        {\n          \"description\": \"Whether the preset is a default preset provided by Elastic Transcoder (<code>System</code>) or a preset that you have defined (<code>Custom</code>).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-preset-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: Preset
---
