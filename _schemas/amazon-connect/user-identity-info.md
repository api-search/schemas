---
description: Contains information about the identity of a user.
layout: schema
name: UserIdentityInfo
properties_list:
- description: The first name.
  name: FirstName
  type: string
- description: The last name.
  name: LastName
  type: string
- description: The email address.
  name: Email
  type: string
- description: The secondary email address.
  name: SecondaryEmail
  type: string
- description: The user's mobile number.
  name: Mobile
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/user-identity-info-schema.json
slug: user-identity-info
source_filename: user-identity-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/user-identity-info-schema.json\",\n  \"title\": \"UserIdentityInfo\",\n  \"description\": \"Contains information about the identity of a user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirstName\": {\n      \"type\": \"string\",\n      \"description\": \"The first name.\",\n      \"example\": \"Jane\"\n    },\n    \"LastName\": {\n      \"type\": \"string\",\n      \"description\": \"The last name.\",\n      \"example\": \"Smith\"\n    },\n    \"Email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"SecondaryEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The secondary email address.\"\n    },\n    \"Mobile\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The user's mobile number.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/user-identity-info-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: UserIdentityInfo
---
