---
description: Represents a call or conference recording captured through the Twilio platform, including duration, status, and storage details.
layout: schema
name: Twilio Recording
properties_list:
- description: Unique 34-character identifier for the recording
  name: sid
  type: string
- description: SID of the Twilio account that created the recording
  name: account_sid
  type: string
- description: SID of the call that was recorded
  name: call_sid
  type: string
- description: SID of the conference if this is a conference recording
  name: conference_sid
  type:
  - string
  - 'null'
- description: Current processing status of the recording
  name: status
  type: string
- description: Number of audio channels (1 for mono, 2 for dual)
  name: channels
  type: integer
- description: How the recording was initiated
  name: source
  type: string
- description: Duration of the recording in seconds
  name: duration
  type:
  - string
  - 'null'
- description: Price of the recording
  name: price
  type:
  - string
  - 'null'
- description: ISO 4217 currency code
  name: price_unit
  type: string
- description: Encryption details if recording encryption is enabled
  name: encryption_details
  type:
  - object
  - 'null'
- description: Error code if the recording failed
  name: error_code
  type:
  - integer
  - 'null'
- description: When the recording started
  name: start_time
  type:
  - string
  - 'null'
- description: ISO 8601 timestamp when the recording was created
  name: date_created
  type: string
- description: ISO 8601 timestamp when the recording was last updated
  name: date_updated
  type: string
- description: Twilio API version used
  name: api_version
  type: string
- description: Relative URI for this recording resource
  name: uri
  type: string
- description: ''
  name: subresource_uris
  type: object
provider_name: Twilio
provider_slug: twilio
schema_file: json-schema/twilio-recording-schema.json
slug: twilio-recording
source_filename: twilio-recording-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.twilio.com/docs/schemas/twilio/recording.json\",\n  \"title\": \"Twilio Recording\",\n  \"description\": \"Represents a call or conference recording captured through the Twilio platform, including duration, status, and storage details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^RE[0-9a-fA-F]{32}$\",\n      \"description\": \"Unique 34-character identifier for the recording\"\n    },\n    \"account_sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^AC[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the Twilio account that created the recording\"\n    },\n    \"call_sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^CA[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the call that was recorded\"\n    },\n    \"conference_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"pattern\"\
  : \"^CF[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the conference if this is a conference recording\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"processing\", \"completed\", \"absent\", \"deleted\", \"failed\"],\n      \"description\": \"Current processing status of the recording\"\n    },\n    \"channels\": {\n      \"type\": \"integer\",\n      \"enum\": [1, 2],\n      \"description\": \"Number of audio channels (1 for mono, 2 for dual)\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DialVerb\",\n        \"Conference\",\n        \"OutboundAPI\",\n        \"Trunking\",\n        \"RecordVerb\",\n        \"StartCallRecordingAPI\",\n        \"StartConferenceRecordingAPI\"\n      ],\n      \"description\": \"How the recording was initiated\"\n    },\n    \"duration\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Duration of the recording in seconds\"\n    },\n    \"price\": {\n      \"\
  type\": [\"string\", \"null\"],\n      \"description\": \"Price of the recording\"\n    },\n    \"price_unit\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"encryption_details\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Encryption details if recording encryption is enabled\",\n      \"properties\": {\n        \"encryption_public_key_sid\": {\n          \"type\": \"string\"\n        },\n        \"type\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"error_code\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Error code if the recording failed\"\n    },\n    \"start_time\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the recording started\"\n    },\n    \"date_created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the recording was\
  \ created\"\n    },\n    \"date_updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the recording was last updated\"\n    },\n    \"api_version\": {\n      \"type\": \"string\",\n      \"description\": \"Twilio API version used\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URI for this recording resource\"\n    },\n    \"subresource_uris\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"transcriptions\": {\n          \"type\": \"string\"\n        },\n        \"add_on_results\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"sid\", \"account_sid\", \"call_sid\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twilio/refs/heads/main/json-schema/twilio-recording-schema.json
tags:
- Authentication
- Communications
- Contact Center
- Email
- IoT
- Messaging
- Phone
- SMS
- T1
- Verification
- Video
- Voice
title: Twilio Recording
---
