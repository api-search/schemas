---
description: An employee user record.
layout: schema
name: User
properties_list:
- description: Unique identifier of the user.
  name: _id
  type: string
- description: Full name of the user.
  name: name
  type: string
- description: Email address of the user.
  name: email
  type: string
- description: ID of the department the user belongs to.
  name: departmentId
  type: string
- description: ID of the location the user is assigned to.
  name: locationId
  type: string
- description: ID of the team the user belongs to.
  name: teamId
  type: string
- description: 'User status: 1=active, 0=inactive.'
  name: status
  type: integer
- description: User's preferred language code.
  name: language
  type: string
provider_name: Absence.io
provider_slug: absence-io
schema_file: json-schema/user-schema.json
slug: user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"An employee user record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the user.\",\n      \"example\": \"500456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the user.\",\n      \"example\": \"Jane Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"departmentId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the department the user belongs to.\",\n      \"example\": \"500999\"\n    },\n    \"locationId\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"ID of the location the user is assigned to.\",\n      \"example\": \"500888\"\n    },\n    \"teamId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the team the user belongs to.\",\n      \"example\": \"500111\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"User status: 1=active, 0=inactive.\",\n      \"example\": 1\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"User's preferred language code.\",\n      \"example\": \"en\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/user-schema.json
tags:
- Absences
- Employees
- Leave Management
- HR
title: User
---
