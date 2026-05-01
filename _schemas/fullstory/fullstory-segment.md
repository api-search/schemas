---
description: A segment in FullStory representing a saved group of users matching specific behavioral criteria. Segments can be used for exports, alerts, and webhook notifications.
layout: schema
name: FullStory Segment
properties_list:
- description: Unique identifier for the segment
  name: id
  type: string
- description: Display name of the segment
  name: name
  type: string
- description: Email address of the FullStory user who created the segment
  name: creator
  type: string
- description: UTC RFC 3339 timestamp for when the segment was created. Not present for built-in segments.
  name: created
  type: string
- description: URL to view the segment in the FullStory application
  name: url
  type: string
provider_name: FullStory
provider_slug: fullstory
schema_file: json-schema/fullstory-segment-schema.json
slug: fullstory-segment
source_filename: fullstory-segment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fullstory.com/schemas/fullstory/segment.json\",\n  \"title\": \"FullStory Segment\",\n  \"description\": \"A segment in FullStory representing a saved group of users matching specific behavioral criteria. Segments can be used for exports, alerts, and webhook notifications.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the segment\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the segment\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the FullStory user who created the segment\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC RFC 3339 timestamp for when\
  \ the segment was created. Not present for built-in segments.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to view the segment in the FullStory application\"\n    }\n  },\n  \"$defs\": {\n    \"SegmentExport\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for exporting segment data\",\n      \"required\": [\"segmentId\", \"type\"],\n      \"properties\": {\n        \"segmentId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the segment to export\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of data to export: individuals for user data or events for behavioral event data\",\n          \"enum\": [\"individuals\", \"events\"]\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"description\": \"The output format for the export\",\n          \"enum\": [\"json\", \"csv\"]\n       \
  \ },\n        \"timeRange\": {\n          \"$ref\": \"#/$defs/TimeRange\",\n          \"description\": \"Optional time range to filter the exported data\"\n        },\n        \"segmentTimeRange\": {\n          \"$ref\": \"#/$defs/TimeRange\",\n          \"description\": \"Optional time range for segment membership evaluation\"\n        }\n      }\n    },\n    \"TimeRange\": {\n      \"type\": \"object\",\n      \"description\": \"A time range defined by start and end timestamps\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Start of the time range in RFC 3339 format\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"End of the time range in RFC 3339 format\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/json-schema/fullstory-segment-schema.json
tags:
- Analytics
- Digital Experience
- Session Replay
- Webhooks
- Data Export
title: FullStory Segment
---
