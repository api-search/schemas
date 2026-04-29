---
description: ''
layout: schema
name: TranscriptionJob
properties_list:
- description: The name of the transcription job.
  name: TranscriptionJobName
  type: string
- description: ''
  name: TranscriptionJobStatus
  type: string
- description: ''
  name: LanguageCode
  type: string
- description: ''
  name: MediaFormat
  type: string
- description: ''
  name: Media
  type: object
- description: ''
  name: Transcript
  type: object
- description: ''
  name: CreationTime
  type: string
- description: ''
  name: CompletionTime
  type: string
provider_name: Amazon Transcribe
provider_slug: amazon-transcribe
schema_file: json-schema/amazon-transcribe-transcription-job-schema.json
slug: amazon-transcribe-transcription-job
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TranscriptionJobName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the transcription job.\"\n    },\n    \"TranscriptionJobStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"QUEUED\",\n        \"IN_PROGRESS\",\n        \"FAILED\",\n        \"COMPLETED\"\n      ]\n    },\n    \"LanguageCode\": {\n      \"type\": \"string\"\n    },\n    \"MediaFormat\": {\n      \"type\": \"string\"\n    },\n    \"Media\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"MediaFileUri\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Transcript\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"TranscriptFileUri\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"CompletionTime\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TranscriptionJob\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-transcribe/refs/heads/main/json-schema/amazon-transcribe-transcription-job-schema.json
tags:
- Audio Processing
- AWS
- Machine Learning
- Speech Recognition
- Speech-To-Text
- Transcription
title: TranscriptionJob
---
