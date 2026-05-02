---
description: A result from the IBM Speech to Text service.
layout: schema
name: Speech Recognition Result
properties_list:
- description: Recognition results.
  name: results
  type: array
- description: The index of the first result.
  name: result_index
  type: integer
- description: Speaker labels for diarization.
  name: speaker_labels
  type: array
provider_name: International Business Machines
provider_slug: international-business-machines
schema_file: json-schema/speech-recognition-result.json
slug: speech-recognition-result
source_filename: speech-recognition-result.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"speech-recognition-result.json\",\n  \"title\": \"Speech Recognition Result\",\n  \"description\": \"A result from the IBM Speech to Text service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Recognition results.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"final\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the result is final.\"\n          },\n          \"alternatives\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"transcript\": {\n                  \"type\": \"string\",\n                  \"description\": \"The transcribed text.\"\n                },\n                \"confidence\": {\n                  \"type\": \"number\",\n\
  \                  \"description\": \"The confidence score.\",\n                  \"minimum\": 0,\n                  \"maximum\": 1\n                }\n              },\n              \"required\": [\"transcript\"]\n            }\n          }\n        }\n      }\n    },\n    \"result_index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the first result.\"\n    },\n    \"speaker_labels\": {\n      \"type\": \"array\",\n      \"description\": \"Speaker labels for diarization.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"from\": { \"type\": \"number\" },\n          \"to\": { \"type\": \"number\" },\n          \"speaker\": { \"type\": \"integer\" },\n          \"confidence\": { \"type\": \"number\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/json-schema/speech-recognition-result.json
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
title: Speech Recognition Result
---
