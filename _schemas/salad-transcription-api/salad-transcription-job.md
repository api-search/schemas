---
description: Schema for a Salad Transcription API job request and response.
layout: schema
name: Salad Transcription Job
properties_list:
- description: Unique identifier for the transcription job.
  name: id
  type: string
- description: Input configuration for the transcription job.
  name: input
  type: object
- description: Optional user-provided metadata attached to the job.
  name: metadata
  type: object
- description: Current status of the transcription job.
  name: status
  type: string
- description: Timeline of job status events.
  name: events
  type: array
- description: Transcription output (available when status is 'succeeded').
  name: output
  type: object
- description: ISO 8601 timestamp when the job was created.
  name: create_time
  type: string
- description: ISO 8601 timestamp of the last job update.
  name: update_time
  type: string
provider_name: Salad Transcription API
provider_slug: salad-transcription-api
schema_file: json-schema/salad-transcription-job-schema.json
slug: salad-transcription-job
source_filename: salad-transcription-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/salad-transcription-api/json-schema/salad-transcription-job-schema.json\",\n  \"title\": \"Salad Transcription Job\",\n  \"description\": \"Schema for a Salad Transcription API job request and response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the transcription job.\",\n      \"example\": \"54e84442-3576-45ca-904c-a1d90bc77baf\"\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"Input configuration for the transcription job.\",\n      \"required\": [\"url\"],\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the audio or video file to transcribe. Must be publicly accessible.\"\n        },\n        \"language_code\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"BCP-47 language code (e.g., 'en', 'fr', 'de'). Defaults to auto-detection.\",\n          \"default\": \"en\",\n          \"example\": \"en\"\n        },\n        \"word_level_timestamps\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to include word-level timestamps in the output.\",\n          \"default\": false\n        },\n        \"diarization\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to identify and separate individual speakers.\",\n          \"default\": false\n        },\n        \"srt\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to generate SRT caption/subtitle output.\",\n          \"default\": false\n        }\n      }\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Optional user-provided metadata attached to the job.\",\n      \"additionalProperties\": true\n    },\n    \"status\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Current status of the transcription job.\",\n      \"enum\": [\"pending\", \"created\", \"running\", \"succeeded\", \"failed\"]\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Timeline of job status events.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"action\": {\n            \"type\": \"string\",\n            \"description\": \"Event action name.\",\n            \"enum\": [\"created\", \"started\", \"succeeded\", \"failed\"]\n          },\n          \"time\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"ISO 8601 timestamp of the event.\"\n          }\n        }\n      }\n    },\n    \"output\": {\n      \"type\": \"object\",\n      \"description\": \"Transcription output (available when status is 'succeeded').\",\n      \"properties\": {\n        \"segments\": {\n          \"type\": \"array\",\n          \"\
  description\": \"Array of transcribed segments.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"start\": { \"type\": \"number\", \"description\": \"Start time in seconds.\" },\n              \"end\": { \"type\": \"number\", \"description\": \"End time in seconds.\" },\n              \"text\": { \"type\": \"string\", \"description\": \"Transcribed text for the segment.\" },\n              \"speaker\": { \"type\": \"string\", \"description\": \"Speaker label (when diarization is enabled).\" },\n              \"words\": {\n                \"type\": \"array\",\n                \"description\": \"Word-level details (when word_level_timestamps is enabled).\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"word\": { \"type\": \"string\" },\n                    \"start\": { \"type\": \"number\" },\n                    \"end\": { \"type\": \"number\"\
  \ },\n                    \"score\": { \"type\": \"number\", \"description\": \"Confidence score (0–1).\" },\n                    \"speaker\": { \"type\": \"string\" }\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"srt_content\": {\n          \"type\": \"string\",\n          \"description\": \"SRT-formatted caption content (when srt is enabled).\"\n        },\n        \"duration\": {\n          \"type\": \"number\",\n          \"description\": \"Total duration of the media in seconds.\"\n        },\n        \"processing_time\": {\n          \"type\": \"number\",\n          \"description\": \"Time taken to process the transcription in seconds.\"\n        }\n      }\n    },\n    \"create_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the job was created.\"\n    },\n    \"update_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n \
  \     \"description\": \"ISO 8601 timestamp of the last job update.\"\n    }\n  },\n  \"required\": [\"input\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salad-transcription-api/refs/heads/main/json-schema/salad-transcription-job-schema.json
tags:
- Audio Transcription
- Captions
- Diarization
- GPU
- Speech Recognition
- Transcription
- Video Processing
title: Salad Transcription Job
---
