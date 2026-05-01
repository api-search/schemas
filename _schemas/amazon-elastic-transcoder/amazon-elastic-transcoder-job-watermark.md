---
description: Watermarks can be in .png or .jpg format. If you want to display a watermark that is not rectangular, use the .png format, which supports transparency.
layout: schema
name: JobWatermark
properties_list:
- description: ''
  name: PresetWatermarkId
  type: object
- description: ''
  name: InputKey
  type: object
- description: ''
  name: Encryption
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-job-watermark-schema.json
slug: amazon-elastic-transcoder-job-watermark
source_filename: amazon-elastic-transcoder-job-watermark-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-watermark-schema.json\",\n  \"title\": \"JobWatermark\",\n  \"description\": \"Watermarks can be in .png or .jpg format. If you want to display a watermark that is not rectangular, use the .png format, which supports transparency.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PresetWatermarkId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PresetWatermarkId\"\n        },\n        {\n          \"description\": \"The ID of the watermark settings that Elastic Transcoder uses to add watermarks to the video during transcoding. The settings are in the preset specified by Preset for the current output. In that preset, the value of Watermarks Id tells Elastic Transcoder which settings to use.\"\n        }\n      ]\n    },\n    \"\
  InputKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WatermarkKey\"\n        },\n        {\n          \"description\": \"<p> The name of the .png or .jpg file that you want to use for the watermark. To determine which Amazon S3 bucket contains the specified file, Elastic Transcoder checks the pipeline specified by <code>Pipeline</code>; the <code>Input Bucket</code> object in that pipeline identifies the bucket.</p> <p> If the file name includes a prefix, for example, <b>logos/128x64.png</b>, include the prefix in the key. If the file isn't in the specified bucket, Elastic Transcoder returns an error. </p>\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Encryption\"\n        },\n        {\n          \"description\": \"The encryption settings, if any, that you want Elastic Transcoder to apply to your watermarks.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-job-watermark-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: JobWatermark
---
