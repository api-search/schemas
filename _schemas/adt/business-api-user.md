---
description: A user with access to a business site.
layout: schema
name: User
properties_list:
- description: Unique user ID.
  name: id
  type: string
- description: Full name of the user.
  name: name
  type: string
- description: Email address.
  name: email
  type: string
- description: User role.
  name: role
  type: string
provider_name: ADT
provider_slug: adt
schema_file: json-schema/business-api-user-schema.json
slug: business-api-user
source_filename: business-api-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"A user with access to a business site.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user ID.\",\n      \"example\": \"usr-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the user.\",\n      \"example\": \"Jane Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"User role.\",\n      \"enum\": [\n        \"admin\",\n        \"manager\",\n        \"employee\",\n        \"contractor\"\n      ],\n      \"example\"\
  : \"employee\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-user-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: User
---
