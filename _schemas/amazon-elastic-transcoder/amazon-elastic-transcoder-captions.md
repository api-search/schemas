---
description: The captions to be created, if any.
layout: schema
name: Captions
properties_list:
- description: ''
  name: MergePolicy
  type: object
- description: ''
  name: CaptionSources
  type: object
- description: ''
  name: CaptionFormats
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-captions-schema.json
slug: amazon-elastic-transcoder-captions
source_filename: amazon-elastic-transcoder-captions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-captions-schema.json\",\n  \"title\": \"Captions\",\n  \"description\": \"The captions to be created, if any.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MergePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionMergePolicy\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"<p>A policy that determines how Elastic Transcoder handles the existence of multiple captions.</p> <ul> <li> <p> <b>MergeOverride:</b> Elastic Transcoder transcodes both embedded and sidecar captions into outputs. If captions for a language are embedded in the input file and also appear in a sidecar file, Elastic Transcoder uses the sidecar captions and ignores the embedded captions for that language.</p> </li>\
  \ <li> <p> <b>MergeRetain:</b> Elastic Transcoder transcodes both embedded and sidecar captions into outputs. If captions for a language are embedded in the input file and also appear in a sidecar file, Elastic Transcoder uses the embedded captions and ignores the sidecar captions for that language. If <code>CaptionSources</code> is empty, Elastic Transcoder omits all sidecar captions from the output files.</p> </li> <li> <p> <b>Override:</b> Elastic Transcoder transcodes only the sidecar captions that you specify in <code>CaptionSources</code>.</p> </li> </ul> <p> <code>MergePolicy</code> cannot be null.</p>\"\n        }\n      ]\n    },\n    \"CaptionSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionSources\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"Source files for the input sidecar captions used during the transcoding process. To omit all sidecar captions, leave <code>CaptionSources</code> blank.\"\
  \n        }\n      ]\n    },\n    \"CaptionFormats\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionFormats\"\n        },\n        {\n          \"description\": \"The array of file formats for the output captions. If you leave this value blank, Elastic Transcoder returns an error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-captions-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: Captions
---
