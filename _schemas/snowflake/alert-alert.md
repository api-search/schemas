---
description: A Snowflake alert
layout: schema
name: Alert
properties_list:
- description: Name of the alert
  name: name
  type: string
- description: user comment associated to an object in the dictionary
  name: comment
  type: string
- description: The warehouse the alert runs in
  name: warehouse
  type: string
- description: The SQL statement that must be evaluated to determine whether to trigger the alert
  name: condition
  type: string
- description: The SQL statement to execute when the alert is triggered
  name: action
  type: string
- description: Date and time when the alert was created.
  name: created_on
  type: string
- description: Database in which the alert is stored
  name: database_name
  type: string
- description: Schema in which the alert is stored
  name: schema_name
  type: string
- description: Role that owns the alert
  name: owner
  type: string
- description: The type of role that owns the alert
  name: owner_role_type
  type: string
- description: The current state of the alert
  name: state
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/alert-alert-schema.json
slug: alert-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Alert\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake alert\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the alert\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"user comment associated to an object in the dictionary\"\n    },\n    \"warehouse\": {\n      \"type\": \"string\",\n      \"description\": \"The warehouse the alert runs in\"\n    },\n    \"condition\": {\n      \"type\": \"string\",\n      \"description\": \"The SQL statement that must be evaluated to determine whether to trigger the alert\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The SQL statement to execute when the alert is triggered\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the alert was created.\"\n    },\n    \"\
  database_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database in which the alert is stored\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"Schema in which the alert is stored\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the alert\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the alert\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the alert\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/alert-alert-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Alert
---
