---
description: Represents a Twilio account or subaccount with configuration details, status, and authentication credentials.
layout: schema
name: Twilio Account
properties_list:
- description: Unique 34-character identifier for the account
  name: sid
  type: string
- description: Human-readable name for the account
  name: friendly_name
  type: string
- description: Current status of the account
  name: status
  type: string
- description: Account type
  name: type
  type: string
- description: Primary authentication token for API access
  name: auth_token
  type: string
- description: SID of the parent account (for subaccounts)
  name: owner_account_sid
  type: string
- description: ISO 8601 timestamp when the account was created
  name: date_created
  type: string
- description: ISO 8601 timestamp when the account was last updated
  name: date_updated
  type: string
- description: Relative URI for this account resource
  name: uri
  type: string
- description: URIs of related subresources
  name: subresource_uris
  type: object
provider_name: Twilio
provider_slug: twilio
schema_file: json-schema/twilio-account-schema.json
slug: twilio-account
source_filename: twilio-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.twilio.com/docs/schemas/twilio/account.json\",\n  \"title\": \"Twilio Account\",\n  \"description\": \"Represents a Twilio account or subaccount with configuration details, status, and authentication credentials.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^AC[0-9a-fA-F]{32}$\",\n      \"description\": \"Unique 34-character identifier for the account\"\n    },\n    \"friendly_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the account\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"suspended\", \"closed\"],\n      \"description\": \"Current status of the account\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"Trial\", \"Full\"],\n      \"description\": \"Account type\"\n    },\n    \"auth_token\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Primary authentication token for API access\"\n    },\n    \"owner_account_sid\": {\n      \"type\": \"string\",\n      \"pattern\": \"^AC[0-9a-fA-F]{32}$\",\n      \"description\": \"SID of the parent account (for subaccounts)\"\n    },\n    \"date_created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the account was created\"\n    },\n    \"date_updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the account was last updated\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URI for this account resource\"\n    },\n    \"subresource_uris\": {\n      \"type\": \"object\",\n      \"description\": \"URIs of related subresources\",\n      \"properties\": {\n        \"available_phone_numbers\": {\n          \"type\": \"string\"\n        },\n        \"calls\"\
  : {\n          \"type\": \"string\"\n        },\n        \"conferences\": {\n          \"type\": \"string\"\n        },\n        \"incoming_phone_numbers\": {\n          \"type\": \"string\"\n        },\n        \"messages\": {\n          \"type\": \"string\"\n        },\n        \"recordings\": {\n          \"type\": \"string\"\n        },\n        \"transcriptions\": {\n          \"type\": \"string\"\n        },\n        \"keys\": {\n          \"type\": \"string\"\n        },\n        \"applications\": {\n          \"type\": \"string\"\n        },\n        \"usage\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"sid\", \"friendly_name\", \"status\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twilio/refs/heads/main/json-schema/twilio-account-schema.json
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
title: Twilio Account
---
