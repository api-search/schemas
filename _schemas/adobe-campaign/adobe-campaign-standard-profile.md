---
description: Profile from Adobe Campaign API
layout: schema
name: Profile
properties_list:
- description: Unique identifier for the profile.
  name: PKey
  type: string
- description: Email address of the profile.
  name: email
  type: string
- description: First name of the profile.
  name: firstName
  type: string
- description: Last name of the profile.
  name: lastName
  type: string
- description: Phone number of the profile.
  name: phone
  type: string
- description: Mobile phone number.
  name: mobilePhone
  type: string
- description: Date of birth.
  name: birthDate
  type: string
- description: Gender of the profile.
  name: gender
  type: string
- description: Preferred language code.
  name: preferredLanguage
  type: string
- description: Whether the profile is on the deny list.
  name: blackList
  type: boolean
- description: Whether email is blocked for this profile.
  name: blackListEmail
  type: boolean
- description: Whether SMS is blocked for this profile.
  name: blackListMobile
  type: boolean
- description: Profile creation timestamp.
  name: created
  type: string
- description: Last modification timestamp.
  name: lastModified
  type: string
- description: Link to the profile subscriptions.
  name: subscriptions
  type: object
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-profile-schema.json
slug: adobe-campaign-standard-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-profile-schema.json\",\n  \"title\": \"Profile\",\n  \"description\": \"Profile from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the profile.\",\n      \"readOnly\": true,\n      \"example\": \"example_value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the profile.\",\n      \"example\": \"user@example.com\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the profile.\",\n      \"example\": \"Example Campaign\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the profile.\",\n      \"\
  example\": \"Example Campaign\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the profile.\",\n      \"example\": \"example_value\"\n    },\n    \"mobilePhone\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number.\",\n      \"example\": \"example_value\"\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of birth.\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"male\",\n        \"female\",\n        \"unknown\"\n      ],\n      \"description\": \"Gender of the profile.\",\n      \"example\": \"male\"\n    },\n    \"preferredLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred language code.\",\n      \"example\": \"example_value\"\n    },\n    \"blackList\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the profile\
  \ is on the deny list.\",\n      \"example\": true\n    },\n    \"blackListEmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether email is blocked for this profile.\",\n      \"example\": true\n    },\n    \"blackListMobile\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether SMS is blocked for this profile.\",\n      \"example\": true\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Profile creation timestamp.\",\n      \"readOnly\": true,\n      \"example\": \"example_value\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp.\",\n      \"readOnly\": true,\n      \"example\": \"example_value\"\n    },\n    \"subscriptions\": {\n      \"type\": \"object\",\n      \"description\": \"Link to the profile subscriptions.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"href\"\
  : {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-profile-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: Profile
---
