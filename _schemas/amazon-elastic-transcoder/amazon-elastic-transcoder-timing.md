---
description: Details about the timing of a job.
layout: schema
name: Timing
properties_list:
- description: ''
  name: SubmitTimeMillis
  type: object
- description: ''
  name: StartTimeMillis
  type: object
- description: ''
  name: FinishTimeMillis
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-timing-schema.json
slug: amazon-elastic-transcoder-timing
source_filename: amazon-elastic-transcoder-timing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-timing-schema.json\",\n  \"title\": \"Timing\",\n  \"description\": \"Details about the timing of a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubmitTimeMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The time the job was submitted to Elastic Transcoder, in epoch milliseconds.\"\n        }\n      ]\n    },\n    \"StartTimeMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The time the job began transcoding, in epoch milliseconds.\"\n        }\n      ]\n    },\n    \"FinishTimeMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The time the job finished transcoding, in epoch milliseconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-timing-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: Timing
---
