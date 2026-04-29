---
description: Provides messages from the service about jobs that you have already successfully submitted.
layout: schema
name: JobMessages
properties_list:
- description: ''
  name: Info
  type: object
- description: ''
  name: Warning
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-job-messages-schema.json
slug: mediaconvert-api-job-messages
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-messages-schema.json\",\n  \"title\": \"JobMessages\",\n  \"description\": \"Provides messages from the service about jobs that you have already successfully submitted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Info\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"info\"\n          },\n          \"description\": \"List of messages that are informational only and don't indicate a problem with your job.\"\n        }\n      ]\n    },\n    \"Warning\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"warning\"\n          },\n         \
  \ \"description\": \"List of messages that warn about conditions that might cause your job not to run or to fail.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-messages-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: JobMessages
---
