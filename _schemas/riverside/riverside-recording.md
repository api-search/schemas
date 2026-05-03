---
description: Schema for a recording session in the Riverside Business API.
layout: schema
name: Riverside Recording
properties_list:
- description: Unique recording identifier
  name: id
  type: string
- description: Recording name
  name: name
  type: string
- description: Identifier of the project this recording belongs to
  name: project_id
  type: string
- description: Name of the project
  name: project_name
  type: string
- description: Identifier of the studio
  name: studio_id
  type: string
- description: Name of the studio
  name: studio_name
  type: string
- description: Processing status of the recording
  name: status
  type: string
- description: Timestamp when the recording was created
  name: created_date
  type: string
- description: Individual audio and video tracks captured during recording
  name: tracks
  type: array
- description: Transcription data for the recording
  name: transcription
  type: object
provider_name: Riverside
provider_slug: riverside
schema_file: json-schema/riverside-recording-schema.json
slug: riverside-recording
source_filename: riverside-recording-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/riverside/json-schema/riverside-recording-schema.json\",\n  \"title\": \"Riverside Recording\",\n  \"description\": \"Schema for a recording session in the Riverside Business API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique recording identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Recording name\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the project this recording belongs to\"\n    },\n    \"project_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the project\"\n    },\n    \"studio_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the studio\"\n    },\n    \"studio_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name\
  \ of the studio\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Processing status of the recording\",\n      \"example\": \"ready\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the recording was created\"\n    },\n    \"tracks\": {\n      \"type\": \"array\",\n      \"description\": \"Individual audio and video tracks captured during recording\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Track identifier\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Track media type (e.g., compressed_audio, raw_video)\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"Track processing status\"\n          },\n          \"files\": {\n       \
  \     \"type\": \"array\",\n            \"description\": \"Downloadable files for this track\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"description\": \"File format type\"\n                },\n                \"size\": {\n                  \"type\": \"integer\",\n                  \"description\": \"File size in bytes\"\n                },\n                \"download_url\": {\n                  \"type\": \"string\",\n                  \"format\": \"uri\",\n                  \"description\": \"Temporary download URL for the file\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"transcription\": {\n      \"type\": \"object\",\n      \"description\": \"Transcription data for the recording\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Transcription processing status\"\n        },\n        \"srt_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to download SRT transcription file\"\n        },\n        \"txt_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to download plain text transcription\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/riverside/refs/heads/main/json-schema/riverside-recording-schema.json
tags:
- Podcast
- Video Recording
- Media
- Content Creation
- Audio
title: Riverside Recording
---
