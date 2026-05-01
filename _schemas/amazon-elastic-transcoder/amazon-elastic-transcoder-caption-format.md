---
description: The file format of the output captions. If you leave this value blank, Elastic Transcoder returns an error.
layout: schema
name: CaptionFormat
properties_list:
- description: ''
  name: Format
  type: object
- description: ''
  name: Pattern
  type: object
- description: ''
  name: Encryption
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-caption-format-schema.json
slug: amazon-elastic-transcoder-caption-format
source_filename: amazon-elastic-transcoder-caption-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-caption-format-schema.json\",\n  \"title\": \"CaptionFormat\",\n  \"description\": \"The file format of the output captions. If you leave this value blank, Elastic Transcoder returns an error.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionFormatFormat\"\n        },\n        {\n          \"description\": \"<p>The format you specify determines whether Elastic Transcoder generates an embedded or sidecar caption for this output.</p> <ul> <li> <p> <b>Valid Embedded Caption Formats:</b> </p> <ul> <li> <p> <b>for FLAC</b>: None</p> </li> <li> <p> <b>For MP3</b>: None</p> </li> <li> <p> <b>For MP4</b>: mov-text</p> </li> <li> <p> <b>For MPEG-TS</b>: None</p> </li> <li> <p>\
  \ <b>For ogg</b>: None</p> </li> <li> <p> <b>For webm</b>: None</p> </li> </ul> </li> <li> <p> <b>Valid Sidecar Caption Formats:</b> Elastic Transcoder supports dfxp (first div element only), scc, srt, and webvtt. If you want ttml or smpte-tt compatible captions, specify dfxp as your output format.</p> <ul> <li> <p> <b>For FMP4</b>: dfxp</p> </li> <li> <p> <b>Non-FMP4 outputs</b>: All sidecar types</p> </li> </ul> <p> <code>fmp4</code> captions have an extension of <code>.ismt</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Pattern\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionFormatPattern\"\n        },\n        {\n          \"description\": \"<p>The prefix for caption filenames, in the form <i>description</i>-<code>{language}</code>, where:</p> <ul> <li> <p> <i>description</i> is a description of the video.</p> </li> <li> <p> <code>{language}</code> is a literal value that Elastic Transcoder replaces with the two- or three-letter\
  \ code for the language of the caption in the output file names.</p> </li> </ul> <p>If you don't include <code>{language}</code> in the file name pattern, Elastic Transcoder automatically appends \\\"<code>{language}</code>\\\" to the value that you specify for the description. In addition, Elastic Transcoder automatically appends the count to the end of the segment files.</p> <p>For example, suppose you're transcoding into srt format. When you enter \\\"Sydney-{language}-sunrise\\\", and the language of the captions is English (en), the name of the first caption file is be Sydney-en-sunrise00000.srt.</p>\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"description\": \"The encryption settings, if any, that you want Elastic Transcoder to apply to your caption formats.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-caption-format-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: CaptionFormat
---
