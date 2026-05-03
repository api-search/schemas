---
description: Represents a voice call made to or from a Twilio account, including call status, duration, pricing, and related metadata.
layout: schema
name: Twilio Call
properties_list:
- description: Unique 34-character identifier for the call
  name: sid
  type: string
- description: SID of the Twilio account that created the call
  name: account_sid
  type: string
- description: SID of the parent call if this is a child call leg
  name: parent_call_sid
  type:
  - string
  - 'null'
- description: Phone number, SIP URI, or client identifier that received the call
  name: to
  type: string
- description: Formatted version of the To number
  name: to_formatted
  type: string
- description: Phone number or client identifier that initiated the call
  name: from
  type: string
- description: Formatted version of the From number
  name: from_formatted
  type: string
- description: SID of the Twilio phone number used
  name: phone_number_sid
  type:
  - string
  - 'null'
- description: Current status of the call
  name: status
  type: string
- description: Direction of the call
  name: direction
  type: string
- description: Price of the call in the account currency
  name: price
  type:
  - string
  - 'null'
- description: ISO 4217 currency code
  name: price_unit
  type: string
- description: Duration of the call in seconds
  name: duration
  type:
  - string
  - 'null'
- description: ISO 8601 timestamp when the call started
  name: start_time
  type:
  - string
  - 'null'
- description: ISO 8601 timestamp when the call ended
  name: end_time
  type:
  - string
  - 'null'
- description: Whether the call was answered by a human or machine
  name: answered_by
  type:
  - string
  - 'null'
- description: Caller name from CNAM lookup
  name: caller_name
  type:
  - string
  - 'null'
- description: Number that forwarded the inbound call
  name: forwarded_from
  type:
  - string
  - 'null'
- description: SID identifying the call group
  name: group_sid
  type:
  - string
  - 'null'
- description: Time the call spent in queue in milliseconds
  name: queue_time
  type:
  - string
  - 'null'
- description: SID of the SIP trunk used for the call
  name: trunk_sid
  type:
  - string
  - 'null'
- description: ISO 8601 timestamp when the resource was created
  name: date_created
  type: string
- description: ISO 8601 timestamp when the resource was last updated
  name: date_updated
  type: string
- description: Twilio API version used
  name: api_version
  type: string
- description: Relative URI for this call resource
  name: uri
  type: string
- description: URIs of related subresources
  name: subresource_uris
  type: object
provider_name: Twilio
provider_slug: twilio
schema_file: json-schema/twilio-call-schema.json
slug: twilio-call
source_filename: twilio-call-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.twilio.com/docs/schemas/twilio/call.json\",\n  \"title\": \"Twilio Call\",\n  \"description\": \"Represents a voice call made to or from a Twilio account, including call status, duration, pricing, and related metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^CA[0-9a-fA-F]{32}$\",\n      \"description\": \"Unique 34-character identifier for the call\"\n    },\n    \"account_sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^AC[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the Twilio account that created the call\"\n    },\n    \"parent_call_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"pattern\": \"^CA[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the parent call if this is a child call leg\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"Phone\
  \ number, SIP URI, or client identifier that received the call\"\n    },\n    \"to_formatted\": {\n      \"type\": \"string\",\n      \"description\": \"Formatted version of the To number\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number or client identifier that initiated the call\"\n    },\n    \"from_formatted\": {\n      \"type\": \"string\",\n      \"description\": \"Formatted version of the From number\"\n    },\n    \"phone_number_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"pattern\": \"^PN[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the Twilio phone number used\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"queued\",\n        \"ringing\",\n        \"in-progress\",\n        \"canceled\",\n        \"completed\",\n        \"failed\",\n        \"busy\",\n        \"no-answer\"\n      ],\n      \"description\": \"Current status of the call\"\n    },\n    \"direction\": {\n   \
  \   \"type\": \"string\",\n      \"enum\": [\n        \"inbound\",\n        \"outbound-api\",\n        \"outbound-dial\"\n      ],\n      \"description\": \"Direction of the call\"\n    },\n    \"price\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Price of the call in the account currency\"\n    },\n    \"price_unit\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"duration\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Duration of the call in seconds\"\n    },\n    \"start_time\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the call started\"\n    },\n    \"end_time\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the call ended\"\n    },\n    \"answered_by\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"human\"\
  , \"machine\", null],\n      \"description\": \"Whether the call was answered by a human or machine\"\n    },\n    \"caller_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Caller name from CNAM lookup\"\n    },\n    \"forwarded_from\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Number that forwarded the inbound call\"\n    },\n    \"group_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"SID identifying the call group\"\n    },\n    \"queue_time\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Time the call spent in queue in milliseconds\"\n    },\n    \"trunk_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"SID of the SIP trunk used for the call\"\n    },\n    \"date_created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the resource was created\"\n    },\n    \"date_updated\": {\n    \
  \  \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the resource was last updated\"\n    },\n    \"api_version\": {\n      \"type\": \"string\",\n      \"description\": \"Twilio API version used\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URI for this call resource\"\n    },\n    \"subresource_uris\": {\n      \"type\": \"object\",\n      \"description\": \"URIs of related subresources\",\n      \"properties\": {\n        \"recordings\": {\n          \"type\": \"string\"\n        },\n        \"notifications\": {\n          \"type\": \"string\"\n        },\n        \"feedback\": {\n          \"type\": \"string\"\n        },\n        \"feedback_summaries\": {\n          \"type\": \"string\"\n        },\n        \"payments\": {\n          \"type\": \"string\"\n        },\n        \"events\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"sid\", \"\
  account_sid\", \"to\", \"from\", \"status\", \"direction\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twilio/refs/heads/main/json-schema/twilio-call-schema.json
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
title: Twilio Call
---
