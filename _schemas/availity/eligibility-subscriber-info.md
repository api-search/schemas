---
description: SubscriberInfo schema from Availity API
layout: schema
name: SubscriberInfo
properties_list:
- description: ''
  name: memberId
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: dateOfBirth
  type: string
- description: ''
  name: gender
  type: string
- description: ''
  name: groupNumber
  type: string
- description: ''
  name: groupName
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-subscriber-info-schema.json
slug: eligibility-subscriber-info
source_filename: eligibility-subscriber-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-subscriber-info-schema.json\",\n  \"title\": \"SubscriberInfo\",\n  \"description\": \"SubscriberInfo schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memberId\": {\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"gender\": {\n      \"type\": \"string\"\n    },\n    \"groupNumber\": {\n      \"type\": \"string\"\n    },\n    \"groupName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-subscriber-info-schema.json
tags: []
title: SubscriberInfo
---
