---
description: Represents a Webex meeting recording including metadata, download links, and playback information.
layout: schema
name: Cisco Webex Recording
properties_list:
- description: Unique identifier for the recording.
  name: id
  type: string
- description: The meeting ID associated with the recording.
  name: meetingId
  type: string
- description: The topic or title of the recording.
  name: topic
  type: string
- description: Date and time the recording was created.
  name: createTime
  type: string
- description: Date and time the recording was made.
  name: timeRecorded
  type: string
- description: URL to download the recording.
  name: downloadUrl
  type: string
- description: URL to play back the recording.
  name: playbackUrl
  type: string
- description: Password required to access the recording.
  name: password
  type: string
- description: Format of the recording file.
  name: format
  type: string
- description: Webex service type the recording originated from.
  name: serviceType
  type: string
- description: Duration of the recording in seconds.
  name: durationSeconds
  type: integer
- description: Size of the recording file in bytes.
  name: sizeBytes
  type: integer
- description: Current status of the recording.
  name: status
  type: string
- description: Temporary download links with expiration timestamps.
  name: temporaryDirectDownloadLinks
  type: object
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-recording-schema.json
slug: cisco-webex-recording
source_filename: cisco-webex-recording-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/recording.json\",\n  \"title\": \"Cisco Webex Recording\",\n  \"description\": \"Represents a Webex meeting recording including metadata, download links, and playback information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the recording.\"\n    },\n    \"meetingId\": {\n      \"type\": \"string\",\n      \"description\": \"The meeting ID associated with the recording.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"The topic or title of the recording.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the recording was created.\"\n    },\n    \"timeRecorded\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Date and time the recording was made.\"\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the recording.\"\n    },\n    \"playbackUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to play back the recording.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password required to access the recording.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Format of the recording file.\",\n      \"enum\": [\"MP4\", \"ARF\", \"UPLOADED\"]\n    },\n    \"serviceType\": {\n      \"type\": \"string\",\n      \"description\": \"Webex service type the recording originated from.\",\n      \"enum\": [\"MeetingCenter\", \"EventCenter\", \"TrainingCenter\", \"SupportCenter\"]\n    },\n    \"durationSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration of the recording in seconds.\"\n\
  \    },\n    \"sizeBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the recording file in bytes.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the recording.\",\n      \"enum\": [\"available\", \"deleted\", \"purged\"]\n    },\n    \"temporaryDirectDownloadLinks\": {\n      \"type\": \"object\",\n      \"description\": \"Temporary download links with expiration timestamps.\",\n      \"properties\": {\n        \"recordingDownloadLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"audioDownloadLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"transcriptDownloadLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"expiration\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-recording-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Recording
---
