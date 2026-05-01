---
description: Represents a prospect in the Gong Engage platform, typically a sales lead or potential customer being targeted through automated outreach flows.
layout: schema
name: Gong Prospect
properties_list:
- description: The prospect's email address.
  name: emailAddress
  type: string
- description: The prospect's first name.
  name: firstName
  type: string
- description: The prospect's last name.
  name: lastName
  type: string
- description: The prospect's company name.
  name: company
  type: string
- description: The prospect's job title.
  name: title
  type: string
- description: The prospect's phone number.
  name: phoneNumber
  type: string
- description: The prospect's LinkedIn profile URL.
  name: linkedInUrl
  type: string
- description: Custom field key-value pairs for the prospect.
  name: customFields
  type: object
provider_name: Gong
provider_slug: gong
schema_file: json-schema/gong-prospect-schema.json
slug: gong-prospect
source_filename: gong-prospect-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gong/blob/main/json-schema/gong-prospect-schema.json\",\n  \"title\": \"Gong Prospect\",\n  \"description\": \"Represents a prospect in the Gong Engage platform, typically a sales lead or potential customer being targeted through automated outreach flows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The prospect's email address.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The prospect's first name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The prospect's last name.\"\n    },\n    \"company\": {\n      \"type\": \"string\",\n      \"description\": \"The prospect's company name.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ prospect's job title.\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The prospect's phone number.\"\n    },\n    \"linkedInUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The prospect's LinkedIn profile URL.\"\n    },\n    \"customFields\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom field key-value pairs for the prospect.\"\n    }\n  },\n  \"required\": [\"emailAddress\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/json-schema/gong-prospect-schema.json
tags: []
title: Gong Prospect
---
