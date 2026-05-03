---
description: Represents a phone number provisioned on the Twilio platform, including capabilities, configuration, and routing settings.
layout: schema
name: Twilio Phone Number
properties_list:
- description: Unique 34-character identifier for the phone number
  name: sid
  type: string
- description: SID of the Twilio account that owns the number
  name: account_sid
  type: string
- description: Human-readable name for the phone number
  name: friendly_name
  type: string
- description: Phone number in E.164 format
  name: phone_number
  type: string
- description: Origin of the phone number
  name: origin
  type: string
- description: Communication capabilities of the number
  name: capabilities
  type: object
- description: URL for TwiML instructions when a call is received
  name: voice_url
  type:
  - string
  - 'null'
- description: HTTP method for the voice URL
  name: voice_method
  type: string
- description: Fallback URL if the voice URL fails
  name: voice_fallback_url
  type:
  - string
  - 'null'
- description: ''
  name: voice_fallback_method
  type: string
- description: Whether to look up caller ID for incoming calls
  name: voice_caller_id_lookup
  type: boolean
- description: URL for handling incoming SMS messages
  name: sms_url
  type:
  - string
  - 'null'
- description: ''
  name: sms_method
  type: string
- description: ''
  name: sms_fallback_url
  type:
  - string
  - 'null'
- description: ''
  name: sms_fallback_method
  type: string
- description: URL for call status change webhooks
  name: status_callback
  type:
  - string
  - 'null'
- description: ''
  name: status_callback_method
  type: string
- description: SID of the TwiML application for voice calls
  name: voice_application_sid
  type:
  - string
  - 'null'
- description: SID of the TwiML application for SMS
  name: sms_application_sid
  type:
  - string
  - 'null'
- description: SID of the SIP trunk associated with this number
  name: trunk_sid
  type:
  - string
  - 'null'
- description: Emergency calling status
  name: emergency_status
  type: string
- description: SID of the emergency address
  name: emergency_address_sid
  type:
  - string
  - 'null'
- description: SID of the address associated with the number
  name: address_sid
  type:
  - string
  - 'null'
- description: SID of the identity resource associated with the number
  name: identity_sid
  type:
  - string
  - 'null'
- description: SID of the regulatory compliance bundle
  name: bundle_sid
  type:
  - string
  - 'null'
- description: Whether the number is a beta (new) number
  name: beta
  type: boolean
- description: ISO 8601 timestamp when the number was provisioned
  name: date_created
  type: string
- description: ISO 8601 timestamp when the number was last updated
  name: date_updated
  type: string
- description: Relative URI for this phone number resource
  name: uri
  type: string
provider_name: Twilio
provider_slug: twilio
schema_file: json-schema/twilio-phone-number-schema.json
slug: twilio-phone-number
source_filename: twilio-phone-number-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.twilio.com/docs/schemas/twilio/phone-number.json\",\n  \"title\": \"Twilio Phone Number\",\n  \"description\": \"Represents a phone number provisioned on the Twilio platform, including capabilities, configuration, and routing settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^PN[0-9a-fA-F]{32}$\",\n      \"description\": \"Unique 34-character identifier for the phone number\"\n    },\n    \"account_sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^AC[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the Twilio account that owns the number\"\n    },\n    \"friendly_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the phone number\"\n    },\n    \"phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number in E.164 format\"\n    },\n\
  \    \"origin\": {\n      \"type\": \"string\",\n      \"enum\": [\"twilio\", \"hosted\"],\n      \"description\": \"Origin of the phone number\"\n    },\n    \"capabilities\": {\n      \"type\": \"object\",\n      \"description\": \"Communication capabilities of the number\",\n      \"properties\": {\n        \"voice\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the number supports voice calls\"\n        },\n        \"sms\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the number supports SMS\"\n        },\n        \"mms\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the number supports MMS\"\n        },\n        \"fax\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the number supports fax\"\n        }\n      }\n    },\n    \"voice_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL for TwiML instructions when a\
  \ call is received\"\n    },\n    \"voice_method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\"],\n      \"description\": \"HTTP method for the voice URL\"\n    },\n    \"voice_fallback_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"Fallback URL if the voice URL fails\"\n    },\n    \"voice_fallback_method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\"]\n    },\n    \"voice_caller_id_lookup\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to look up caller ID for incoming calls\"\n    },\n    \"sms_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL for handling incoming SMS messages\"\n    },\n    \"sms_method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\"]\n    },\n    \"sms_fallback_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\"\n    },\n    \"sms_fallback_method\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\"]\n    },\n    \"status_callback\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL for call status change webhooks\"\n    },\n    \"status_callback_method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\"]\n    },\n    \"voice_application_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"pattern\": \"^AP[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the TwiML application for voice calls\"\n    },\n    \"sms_application_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"pattern\": \"^AP[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the TwiML application for SMS\"\n    },\n    \"trunk_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"SID of the SIP trunk associated with this number\"\n    },\n    \"emergency_status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\"],\n\
  \      \"description\": \"Emergency calling status\"\n    },\n    \"emergency_address_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"SID of the emergency address\"\n    },\n    \"address_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"SID of the address associated with the number\"\n    },\n    \"identity_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"SID of the identity resource associated with the number\"\n    },\n    \"bundle_sid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"SID of the regulatory compliance bundle\"\n    },\n    \"beta\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the number is a beta (new) number\"\n    },\n    \"date_created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the number was provisioned\"\n    },\n    \"date_updated\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the number was last updated\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URI for this phone number resource\"\n    }\n  },\n  \"required\": [\"sid\", \"account_sid\", \"phone_number\", \"capabilities\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twilio/refs/heads/main/json-schema/twilio-phone-number-schema.json
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
title: Twilio Phone Number
---
