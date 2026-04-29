---
description: ProfileUpdate from Adobe Campaign API
layout: schema
name: ProfileUpdate
properties_list:
- description: ''
  name: email
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: mobilePhone
  type: string
- description: ''
  name: birthDate
  type: string
- description: ''
  name: gender
  type: string
- description: ''
  name: preferredLanguage
  type: string
- description: ''
  name: blackList
  type: boolean
- description: ''
  name: blackListEmail
  type: boolean
- description: ''
  name: blackListMobile
  type: boolean
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-profile-update-schema.json
slug: adobe-campaign-standard-profile-update
source_filename: adobe-campaign-standard-profile-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-profile-update-schema.json\",\n  \"title\": \"ProfileUpdate\",\n  \"description\": \"ProfileUpdate from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\": \"user@example.com\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"Example Campaign\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"Example Campaign\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"mobilePhone\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"\
  2026-04-17T12:00:00Z\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"male\",\n        \"female\",\n        \"unknown\"\n      ],\n      \"example\": \"male\"\n    },\n    \"preferredLanguage\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"blackList\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"blackListEmail\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"blackListMobile\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-profile-update-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: ProfileUpdate
---
