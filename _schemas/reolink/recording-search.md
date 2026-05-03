---
description: Search parameters and results for querying recorded video files by date, time range, channel, and stream type.
layout: schema
name: Reolink Recording Search
properties_list:
- description: Camera channel number to search
  name: channel
  type: integer
- description: 0 for full results with file details, 1 for recording status bitmask only
  name: onlyStatus
  type: integer
- description: Stream type to search
  name: streamType
  type: string
- description: Search range start time
  name: StartTime
  type: object
- description: Search range end time
  name: EndTime
  type: object
provider_name: Reolink
provider_slug: reolink
schema_file: json-schema/recording-search.json
slug: recording-search
source_filename: recording-search.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"recording-search.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reolink Recording Search\",\n  \"description\": \"Search parameters and results for querying recorded video files by date, time range, channel, and stream type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"type\": \"integer\",\n      \"description\": \"Camera channel number to search\",\n      \"minimum\": 0\n    },\n    \"onlyStatus\": {\n      \"type\": \"integer\",\n      \"description\": \"0 for full results with file details, 1 for recording status bitmask only\",\n      \"enum\": [0, 1]\n    },\n    \"streamType\": {\n      \"type\": \"string\",\n      \"description\": \"Stream type to search\",\n      \"enum\": [\"main\", \"sub\"]\n    },\n    \"StartTime\": {\n      \"$ref\": \"#/$defs/TimeStamp\",\n      \"description\": \"Search range start time\"\n    },\n    \"EndTime\": {\n      \"$ref\": \"#/$defs/TimeStamp\"\
  ,\n      \"description\": \"Search range end time\"\n    }\n  },\n  \"required\": [\"channel\", \"onlyStatus\", \"streamType\", \"StartTime\", \"EndTime\"],\n  \"$defs\": {\n    \"TimeStamp\": {\n      \"type\": \"object\",\n      \"description\": \"Date and time components\",\n      \"properties\": {\n        \"year\": {\n          \"type\": \"integer\",\n          \"description\": \"Year (e.g., 2026)\"\n        },\n        \"mon\": {\n          \"type\": \"integer\",\n          \"description\": \"Month (1-12)\",\n          \"minimum\": 1,\n          \"maximum\": 12\n        },\n        \"day\": {\n          \"type\": \"integer\",\n          \"description\": \"Day of month (1-31)\",\n          \"minimum\": 1,\n          \"maximum\": 31\n        },\n        \"hour\": {\n          \"type\": \"integer\",\n          \"description\": \"Hour (0-23)\",\n          \"minimum\": 0,\n          \"maximum\": 23\n        },\n        \"min\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Minute (0-59)\",\n          \"minimum\": 0,\n          \"maximum\": 59\n        },\n        \"sec\": {\n          \"type\": \"integer\",\n          \"description\": \"Second (0-59)\",\n          \"minimum\": 0,\n          \"maximum\": 59\n        }\n      },\n      \"required\": [\"year\", \"mon\", \"day\", \"hour\", \"min\", \"sec\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/json-schema/recording-search.json
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
title: Reolink Recording Search
---
