---
description: Represents a user account in the Gong platform, including profile information, settings, and organizational details.
layout: schema
name: Gong User
properties_list:
- description: Unique Gong user identifier.
  name: id
  type: string
- description: The user's email address.
  name: emailAddress
  type: string
- description: The user's first name.
  name: firstName
  type: string
- description: The user's last name.
  name: lastName
  type: string
- description: The user's job title.
  name: title
  type: string
- description: The user's phone number.
  name: phoneNumber
  type: string
- description: The user's phone extension.
  name: extension
  type: string
- description: List of the user's personal meeting URLs.
  name: personalMeetingUrls
  type: array
- description: User recording and import settings.
  name: settings
  type: object
- description: The Gong user ID of this user's manager.
  name: managerId
  type: string
- description: URL of the meeting consent page.
  name: meetingConsentPageUrl
  type: string
- description: Languages spoken by the user.
  name: spokenLanguages
  type: array
- description: Whether the user account is active.
  name: active
  type: boolean
- description: When the user account was created.
  name: created
  type: string
- description: URL of the user's avatar image.
  name: avatarUrl
  type: string
- description: The user's trusted email address for SSO.
  name: trustedEmailAddress
  type: string
provider_name: Gong
provider_slug: gong
schema_file: json-schema/gong-user-schema.json
slug: gong-user
source_filename: gong-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gong/blob/main/json-schema/gong-user-schema.json\",\n  \"title\": \"Gong User\",\n  \"description\": \"Represents a user account in the Gong platform, including profile information, settings, and organizational details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Gong user identifier.\"\n    },\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The user's email address.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's first name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's last name.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The user's job title.\"\n    },\n    \"phoneNumber\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The user's phone number.\"\n    },\n    \"extension\": {\n      \"type\": \"string\",\n      \"description\": \"The user's phone extension.\"\n    },\n    \"personalMeetingUrls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"List of the user's personal meeting URLs.\"\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"User recording and import settings.\",\n      \"properties\": {\n        \"webConferencesRecorded\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether web conferences are recorded.\"\n        },\n        \"preventWebConferenceRecording\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether web conference recording is prevented.\"\n        },\n        \"telephonyCallsImported\": {\n          \"type\": \"boolean\",\n          \"description\":\
  \ \"Whether telephony calls are imported.\"\n        },\n        \"emailsImported\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether emails are imported.\"\n        },\n        \"preventEmailImport\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether email import is prevented.\"\n        }\n      }\n    },\n    \"managerId\": {\n      \"type\": \"string\",\n      \"description\": \"The Gong user ID of this user's manager.\"\n    },\n    \"meetingConsentPageUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the meeting consent page.\"\n    },\n    \"spokenLanguages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"language\": {\n            \"type\": \"string\"\n          },\n          \"primary\": {\n            \"type\": \"boolean\"\n          }\n        }\n      },\n      \"description\": \"Languages spoken by the\
  \ user.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is active.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the user account was created.\"\n    },\n    \"avatarUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the user's avatar image.\"\n    },\n    \"trustedEmailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The user's trusted email address for SSO.\"\n    }\n  },\n  \"required\": [\"id\", \"emailAddress\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/json-schema/gong-user-schema.json
tags: []
title: Gong User
---
