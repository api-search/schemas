---
description: Represents a verification request sent through the Twilio Verify API, including the channel used, delivery status, and code attempt history.
layout: schema
name: Twilio Verification
properties_list:
- description: Unique 34-character identifier for the verification
  name: sid
  type: string
- description: SID of the Verify service
  name: service_sid
  type: string
- description: SID of the Twilio account
  name: account_sid
  type: string
- description: Phone number or email address being verified
  name: to
  type: string
- description: Delivery channel used for the verification code
  name: channel
  type: string
- description: Current status of the verification
  name: status
  type: string
- description: Whether the verification was successfully validated
  name: valid
  type: boolean
- description: Phone number lookup data if enabled on the service
  name: lookup
  type:
  - object
  - 'null'
- description: Amount for PSD2 verification
  name: amount
  type:
  - string
  - 'null'
- description: Payee for PSD2 verification
  name: payee
  type:
  - string
  - 'null'
- description: List of code delivery attempts
  name: send_code_attempts
  type: array
- description: ISO 8601 timestamp when the verification was created
  name: date_created
  type: string
- description: ISO 8601 timestamp when the verification was last updated
  name: date_updated
  type: string
- description: Absolute URL of this verification resource
  name: url
  type: string
provider_name: Twilio
provider_slug: twilio
schema_file: json-schema/twilio-verification-schema.json
slug: twilio-verification
source_filename: twilio-verification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.twilio.com/docs/schemas/twilio/verification.json\",\n  \"title\": \"Twilio Verification\",\n  \"description\": \"Represents a verification request sent through the Twilio Verify API, including the channel used, delivery status, and code attempt history.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^VE[0-9a-fA-F]{32}$\",\n      \"description\": \"Unique 34-character identifier for the verification\"\n    },\n    \"service_sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^VA[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the Verify service\"\n    },\n    \"account_sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^AC[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the Twilio account\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number or email address\
  \ being verified\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"enum\": [\"sms\", \"call\", \"email\", \"whatsapp\", \"sna\"],\n      \"description\": \"Delivery channel used for the verification code\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"approved\",\n        \"canceled\",\n        \"max_attempts_reached\",\n        \"deleted\",\n        \"failed\",\n        \"expired\"\n      ],\n      \"description\": \"Current status of the verification\"\n    },\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the verification was successfully validated\"\n    },\n    \"lookup\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Phone number lookup data if enabled on the service\",\n      \"properties\": {\n        \"carrier\": {\n          \"type\": [\"object\", \"null\"],\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\"\
  ,\n              \"description\": \"Line type (mobile, landline, voip, etc.)\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Carrier name\"\n            },\n            \"mobile_country_code\": {\n              \"type\": \"string\"\n            },\n            \"mobile_network_code\": {\n              \"type\": \"string\"\n            },\n            \"error_code\": {\n              \"type\": [\"integer\", \"null\"]\n            }\n          }\n        }\n      }\n    },\n    \"amount\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Amount for PSD2 verification\"\n    },\n    \"payee\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Payee for PSD2 verification\"\n    },\n    \"send_code_attempts\": {\n      \"type\": \"array\",\n      \"description\": \"List of code delivery attempts\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"\
  attempt_sid\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the attempt\"\n          },\n          \"channel\": {\n            \"type\": \"string\",\n            \"description\": \"Channel used for this attempt\"\n          },\n          \"time\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"When the attempt was made\"\n          }\n        }\n      }\n    },\n    \"date_created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the verification was created\"\n    },\n    \"date_updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the verification was last updated\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Absolute URL of this verification resource\"\n    }\n  },\n  \"required\"\
  : [\"sid\", \"service_sid\", \"account_sid\", \"to\", \"channel\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twilio/refs/heads/main/json-schema/twilio-verification-schema.json
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
title: Twilio Verification
---
