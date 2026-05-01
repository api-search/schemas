---
description: Schema for a Google Cloud Video Intelligence annotation request.
layout: schema
name: Video Annotation Request
properties_list:
- description: Google Cloud Storage URI of the video to annotate.
  name: inputUri
  type: string
- description: Base64-encoded video content for inline processing.
  name: inputContent
  type: string
- description: The video analysis features to enable.
  name: features
  type: array
- description: Additional video context and configuration.
  name: videoContext
  type: object
- description: Google Cloud Storage URI for output results.
  name: outputUri
  type: string
- description: Cloud region where annotation should take place.
  name: locationId
  type: string
provider_name: Google Cloud Video Intelligence
provider_slug: google-cloud-video-intelligence
schema_file: json-schema/video-annotation.json
slug: video-annotation
source_filename: video-annotation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-video-intelligence/refs/heads/main/json-schema/video-annotation.json\",\n  \"title\": \"Video Annotation Request\",\n  \"description\": \"Schema for a Google Cloud Video Intelligence annotation request.\",\n  \"type\": \"object\",\n  \"required\": [\"features\"],\n  \"properties\": {\n    \"inputUri\": {\n      \"type\": \"string\",\n      \"description\": \"Google Cloud Storage URI of the video to annotate.\"\n    },\n    \"inputContent\": {\n      \"type\": \"string\",\n      \"description\": \"Base64-encoded video content for inline processing.\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"The video analysis features to enable.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"FEATURE_UNSPECIFIED\",\n          \"LABEL_DETECTION\",\n          \"SHOT_CHANGE_DETECTION\"\
  ,\n          \"EXPLICIT_CONTENT_DETECTION\",\n          \"SPEECH_TRANSCRIPTION\",\n          \"TEXT_DETECTION\",\n          \"OBJECT_TRACKING\",\n          \"LOGO_RECOGNITION\",\n          \"PERSON_DETECTION\"\n        ]\n      }\n    },\n    \"videoContext\": {\n      \"type\": \"object\",\n      \"description\": \"Additional video context and configuration.\",\n      \"properties\": {\n        \"segments\": {\n          \"type\": \"array\",\n          \"description\": \"Video segments to annotate.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"startTimeOffset\": {\n                \"type\": \"string\",\n                \"description\": \"Start time offset in seconds.\"\n              },\n              \"endTimeOffset\": {\n                \"type\": \"string\",\n                \"description\": \"End time offset in seconds.\"\n              }\n            }\n          }\n        },\n        \"labelDetectionConfig\": {\n  \
  \        \"type\": \"object\",\n          \"properties\": {\n            \"labelDetectionMode\": {\n              \"type\": \"string\",\n              \"enum\": [\"LABEL_DETECTION_MODE_UNSPECIFIED\", \"SHOT_MODE\", \"FRAME_MODE\", \"SHOT_AND_FRAME_MODE\"]\n            },\n            \"stationaryCamera\": {\n              \"type\": \"boolean\"\n            },\n            \"model\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"outputUri\": {\n      \"type\": \"string\",\n      \"description\": \"Google Cloud Storage URI for output results.\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud region where annotation should take place.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-video-intelligence/refs/heads/main/json-schema/video-annotation.json
tags:
- Content Moderation
- Google Cloud
- Machine Learning
- Object Detection
- Video Analysis
- Video Intelligence
title: Video Annotation Request
---
