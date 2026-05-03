---
description: Represents an SMS or MMS message sent or received through the Twilio Messaging API, including delivery status, pricing, and metadata.
layout: schema
name: Twilio Message
properties_list:
- description: Unique 34-character identifier for the message (SM for SMS, MM for MMS)
  name: sid
  type: string
- description: SID of the Twilio account that created the message
  name: account_sid
  type: string
- description: SID of the messaging service used to send the message
  name: messaging_service_sid
  type:
  - string
  - 'null'
- description: Recipient phone number in E.164 format
  name: to
  type: string
- description: Sender phone number, short code, or alphanumeric sender ID
  name: from
  type: string
- description: Text content of the message (up to 1600 characters)
  name: body
  type:
  - string
  - 'null'
- description: Current delivery status of the message
  name: status
  type: string
- description: Direction of the message relative to your Twilio account
  name: direction
  type: string
- description: Number of segments the message body was split into
  name: num_segments
  type: string
- description: Number of media files associated with the message
  name: num_media
  type: string
- description: Price of the message in the account currency
  name: price
  type:
  - string
  - 'null'
- description: ISO 4217 currency code for the price
  name: price_unit
  type: string
- description: Twilio error code if the message failed
  name: error_code
  type:
  - integer
  - 'null'
- description: Human-readable description of the error
  name: error_message
  type:
  - string
  - 'null'
- description: ISO 8601 timestamp when the message resource was created
  name: date_created
  type: string
- description: ISO 8601 timestamp when the message was last updated
  name: date_updated
  type: string
- description: ISO 8601 timestamp when the message was sent
  name: date_sent
  type:
  - string
  - 'null'
- description: Twilio API version used to process the message
  name: api_version
  type: string
- description: Relative URI for this message resource
  name: uri
  type: string
- description: URIs of related subresources
  name: subresource_uris
  type: object
provider_name: Twilio
provider_slug: twilio
schema_file: json-schema/twilio-message-schema.json
slug: twilio-message
source_filename: twilio-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.twilio.com/docs/schemas/twilio/message.json\",\n  \"title\": \"Twilio Message\",\n  \"description\": \"Represents an SMS or MMS message sent or received through the Twilio Messaging API, including delivery status, pricing, and metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^(SM|MM)[0-9a-fA-F]{32}$\",\n      \"description\": \"Unique 34-character identifier for the message (SM for SMS, MM for MMS)\"\n    },\n    \"account_sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^AC[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the Twilio account that created the message\"\n    },\n    \"messaging_service_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"pattern\": \"^MG[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the messaging service used to send the message\"\n    },\n    \"to\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Recipient phone number in E.164 format\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"Sender phone number, short code, or alphanumeric sender ID\"\n    },\n    \"body\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 1600,\n      \"description\": \"Text content of the message (up to 1600 characters)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"queued\",\n        \"sending\",\n        \"sent\",\n        \"delivered\",\n        \"undelivered\",\n        \"failed\",\n        \"receiving\",\n        \"received\",\n        \"accepted\",\n        \"scheduled\",\n        \"read\",\n        \"partially_delivered\",\n        \"canceled\"\n      ],\n      \"description\": \"Current delivery status of the message\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"inbound\",\n        \"outbound-api\",\n  \
  \      \"outbound-call\",\n        \"outbound-reply\"\n      ],\n      \"description\": \"Direction of the message relative to your Twilio account\"\n    },\n    \"num_segments\": {\n      \"type\": \"string\",\n      \"description\": \"Number of segments the message body was split into\"\n    },\n    \"num_media\": {\n      \"type\": \"string\",\n      \"description\": \"Number of media files associated with the message\"\n    },\n    \"price\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Price of the message in the account currency\"\n    },\n    \"price_unit\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the price\"\n    },\n    \"error_code\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Twilio error code if the message failed\"\n    },\n    \"error_message\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Human-readable description of the error\"\n    },\n    \"date_created\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the message resource was created\"\n    },\n    \"date_updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the message was last updated\"\n    },\n    \"date_sent\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the message was sent\"\n    },\n    \"api_version\": {\n      \"type\": \"string\",\n      \"description\": \"Twilio API version used to process the message\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URI for this message resource\"\n    },\n    \"subresource_uris\": {\n      \"type\": \"object\",\n      \"description\": \"URIs of related subresources\",\n      \"properties\": {\n        \"media\": {\n          \"type\": \"string\",\n          \"description\": \"URI\
  \ for associated media resources\"\n        },\n        \"feedback\": {\n          \"type\": \"string\",\n          \"description\": \"URI for message feedback\"\n        }\n      }\n    }\n  },\n  \"required\": [\"sid\", \"account_sid\", \"to\", \"from\", \"status\", \"direction\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twilio/refs/heads/main/json-schema/twilio-message-schema.json
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
title: Twilio Message
---
