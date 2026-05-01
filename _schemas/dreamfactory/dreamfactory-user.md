---
description: A user account in a DreamFactory instance, representing a non-admin consumer who authenticates via email and password and is governed by role-based access control.
layout: schema
name: DreamFactory User
properties_list:
- description: Unique identifier for the user.
  name: id
  type: integer
- description: Display name of the user.
  name: name
  type: string
- description: First name of the user.
  name: first_name
  type: string
- description: Last name of the user.
  name: last_name
  type: string
- description: Email address used for login.
  name: email
  type: string
- description: Whether the user account is active.
  name: is_active
  type: boolean
- description: Phone number of the user.
  name: phone
  type: string
- description: Timestamp when the user was created.
  name: created_date
  type: string
- description: Timestamp when the user was last modified.
  name: last_modified_date
  type: string
provider_name: DreamFactory
provider_slug: dreamfactory
schema_file: json-schema/dreamfactory-user.json
slug: dreamfactory-user
source_filename: dreamfactory-user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-user.json\",\n  \"title\": \"DreamFactory User\",\n  \"description\": \"A user account in a DreamFactory instance, representing a non-admin consumer who authenticates via email and password and is governed by role-based access control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the user.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the user.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\
  ,\n      \"description\": \"Email address used for login.\"\n    },\n    \"is_active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is active.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the user.\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user was created.\"\n    },\n    \"last_modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the user was last modified.\"\n    }\n  },\n  \"required\": [\n    \"email\",\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-user.json
tags:
- Automation
- Deployment
- Documentation
- Generation
- Security
title: DreamFactory User
---
