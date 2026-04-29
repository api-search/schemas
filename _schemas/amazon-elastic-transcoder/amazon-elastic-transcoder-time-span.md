---
description: Settings that determine when a clip begins and how long it lasts.
layout: schema
name: TimeSpan
properties_list:
- description: ''
  name: StartTime
  type: object
- description: ''
  name: Duration
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-time-span-schema.json
slug: amazon-elastic-transcoder-time-span
source_filename: amazon-elastic-transcoder-time-span-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-time-span-schema.json\",\n  \"title\": \"TimeSpan\",\n  \"description\": \"Settings that determine when a clip begins and how long it lasts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"The place in the input file where you want a clip to start. The format can be either HH:mm:ss.SSS (maximum value: 23:59:59.999; SSS is thousandths of a second) or sssss.SSS (maximum value: 86399.999). If you don't specify a value, Elastic Transcoder starts at the beginning of the input file.\"\n        }\n      ]\n    },\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n  \
  \      },\n        {\n          \"description\": \"<p>The duration of the clip. The format can be either HH:mm:ss.SSS (maximum value: 23:59:59.999; SSS is thousandths of a second) or sssss.SSS (maximum value: 86399.999). If you don't specify a value, Elastic Transcoder creates an output file from StartTime to the end of the file.</p> <p>If you specify a value longer than the duration of the input file, Elastic Transcoder transcodes the file and returns a warning message.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-time-span-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: TimeSpan
---
