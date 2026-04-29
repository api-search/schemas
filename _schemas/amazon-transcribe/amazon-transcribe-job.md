---
description: Schema representing an Amazon Transcribe transcription job resource.
layout: schema
name: Amazon Transcribe Transcription Job
properties_list:
- description: The name of the transcription job.
  name: TranscriptionJobName
  type: string
- description: The status of the transcription job.
  name: TranscriptionJobStatus
  type: string
- description: The language code for the input audio.
  name: LanguageCode
  type: string
- description: The sample rate of the input audio in Hz.
  name: MediaSampleRateHertz
  type: integer
- description: The format of the input media file.
  name: MediaFormat
  type: string
- description: The location of the input media file.
  name: Media
  type: object
- description: The location of the transcription output.
  name: Transcript
  type: object
- description: Optional settings for the transcription job.
  name: Settings
  type: object
- description: A timestamp indicating when the job was created.
  name: CreationTime
  type: string
- description: A timestamp indicating when the job started processing.
  name: StartTime
  type: string
- description: A timestamp indicating when the job was completed.
  name: CompletionTime
  type: string
- description: The reason the job failed, if applicable.
  name: FailureReason
  type: string
- description: A list of tags associated with the transcription job.
  name: Tags
  type: array
provider_name: Amazon Transcribe
provider_slug: amazon-transcribe
schema_file: json-schema/amazon-transcribe-job-schema.json
slug: amazon-transcribe-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://transcribe.amazonaws.com/schemas/transcription-job\",\n  \"title\": \"Amazon Transcribe Transcription Job\",\n  \"description\": \"Schema representing an Amazon Transcribe transcription job resource.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"TranscriptionJobName\",\n    \"Media\"\n  ],\n  \"properties\": {\n    \"TranscriptionJobName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the transcription job.\",\n      \"minLength\": 1,\n      \"maxLength\": 200,\n      \"pattern\": \"^[0-9a-zA-Z._-]+$\"\n    },\n    \"TranscriptionJobStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the transcription job.\",\n      \"enum\": [\n        \"QUEUED\",\n        \"IN_PROGRESS\",\n        \"FAILED\",\n        \"COMPLETED\"\n      ]\n    },\n    \"LanguageCode\": {\n      \"type\": \"string\",\n      \"description\": \"The language\
  \ code for the input audio.\",\n      \"pattern\": \"^[a-z]{2}-[A-Z]{2}$\"\n    },\n    \"MediaSampleRateHertz\": {\n      \"type\": \"integer\",\n      \"description\": \"The sample rate of the input audio in Hz.\",\n      \"minimum\": 8000,\n      \"maximum\": 48000\n    },\n    \"MediaFormat\": {\n      \"type\": \"string\",\n      \"description\": \"The format of the input media file.\",\n      \"enum\": [\n        \"mp3\",\n        \"mp4\",\n        \"wav\",\n        \"flac\",\n        \"ogg\",\n        \"amr\",\n        \"webm\"\n      ]\n    },\n    \"Media\": {\n      \"type\": \"object\",\n      \"description\": \"The location of the input media file.\",\n      \"required\": [\n        \"MediaFileUri\"\n      ],\n      \"properties\": {\n        \"MediaFileUri\": {\n          \"type\": \"string\",\n          \"description\": \"The S3 location of the input media file.\",\n          \"maxLength\": 2000,\n          \"pattern\": \"^(s3|https)://.*$\"\n        },\n        \"RedactedMediaFileUri\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The S3 location of the redacted media file.\"\n        }\n      }\n    },\n    \"Transcript\": {\n      \"type\": \"object\",\n      \"description\": \"The location of the transcription output.\",\n      \"properties\": {\n        \"TranscriptFileUri\": {\n          \"type\": \"string\",\n          \"description\": \"The S3 location of the transcription output.\"\n        },\n        \"RedactedTranscriptFileUri\": {\n          \"type\": \"string\",\n          \"description\": \"The S3 location of the redacted transcription output.\"\n        }\n      }\n    },\n    \"Settings\": {\n      \"type\": \"object\",\n      \"description\": \"Optional settings for the transcription job.\",\n      \"properties\": {\n        \"VocabularyName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of a vocabulary to use for transcription.\"\n        },\n        \"ShowSpeakerLabels\": {\n          \"type\": \"\
  boolean\",\n          \"description\": \"Whether to identify different speakers in the audio.\"\n        },\n        \"MaxSpeakerLabels\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of speakers to identify.\",\n          \"minimum\": 2,\n          \"maximum\": 10\n        },\n        \"ShowAlternatives\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to show alternative transcriptions.\"\n        },\n        \"MaxAlternatives\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of alternative transcriptions.\",\n          \"minimum\": 2,\n          \"maximum\": 10\n        }\n      }\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp indicating when the job was created.\"\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp indicating\
  \ when the job started processing.\"\n    },\n    \"CompletionTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp indicating when the job was completed.\"\n    },\n    \"FailureReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the job failed, if applicable.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of tags associated with the transcription job.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      },\n      \"maxItems\": 200\n    }\n  },\n  \"$defs\": {\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair for tagging resources.\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"description\": \"The tag key.\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The tag value.\",\n          \"minLength\": 0,\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-transcribe/refs/heads/main/json-schema/amazon-transcribe-job-schema.json
tags:
- Audio Processing
- AWS
- Machine Learning
- Speech Recognition
- Speech-To-Text
- Transcription
title: Amazon Transcribe Transcription Job
---
