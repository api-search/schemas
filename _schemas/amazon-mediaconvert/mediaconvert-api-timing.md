---
description: Information about when jobs are submitted, started, and finished is specified in Unix epoch format in seconds.
layout: schema
name: Timing
properties_list:
- description: ''
  name: FinishTime
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: SubmitTime
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-timing-schema.json
slug: mediaconvert-api-timing
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timing-schema.json\",\n  \"title\": \"Timing\",\n  \"description\": \"Information about when jobs are submitted, started, and finished is specified in Unix epoch format in seconds.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FinishTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"finishTime\"\n          },\n          \"description\": \"The time, in Unix epoch format, that the transcoding job finished\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startTime\"\n          },\n          \"\
  description\": \"The time, in Unix epoch format, that transcoding for the job began.\"\n        }\n      ]\n    },\n    \"SubmitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"submitTime\"\n          },\n          \"description\": \"The time, in Unix epoch format, that you submitted the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timing-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Timing
---
