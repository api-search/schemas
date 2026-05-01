---
description: Represents a call transcript in the Gong platform, containing speaker-identified segments with timing information.
layout: schema
name: Gong Call Transcript
properties_list:
- description: The call ID this transcript belongs to.
  name: callId
  type: string
- description: Transcript segments with speaker and timing data.
  name: transcript
  type: array
provider_name: Gong
provider_slug: gong
schema_file: json-schema/gong-transcript-schema.json
slug: gong-transcript
source_filename: gong-transcript-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gong/blob/main/json-schema/gong-transcript-schema.json\",\n  \"title\": \"Gong Call Transcript\",\n  \"description\": \"Represents a call transcript in the Gong platform, containing speaker-identified segments with timing information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callId\": {\n      \"type\": \"string\",\n      \"description\": \"The call ID this transcript belongs to.\"\n    },\n    \"transcript\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TranscriptSegment\"\n      },\n      \"description\": \"Transcript segments with speaker and timing data.\"\n    }\n  },\n  \"required\": [\"callId\"],\n  \"$defs\": {\n    \"TranscriptSegment\": {\n      \"type\": \"object\",\n      \"description\": \"A segment of a call transcript attributed to a specific speaker.\",\n      \"properties\": {\n        \"speakerId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"ID of the speaker.\"\n        },\n        \"topic\": {\n          \"type\": \"string\",\n          \"description\": \"Topic of the segment.\"\n        },\n        \"sentences\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/TranscriptSentence\"\n          },\n          \"description\": \"Individual sentences within the segment.\"\n        }\n      }\n    },\n    \"TranscriptSentence\": {\n      \"type\": \"object\",\n      \"description\": \"A single transcribed sentence with timing information.\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"number\",\n          \"description\": \"Start time in seconds.\"\n        },\n        \"end\": {\n          \"type\": \"number\",\n          \"description\": \"End time in seconds.\"\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"The transcribed text.\"\n        }\n\
  \      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/json-schema/gong-transcript-schema.json
tags: []
title: Gong Call Transcript
---
