---
description: A system administrator account in a DreamFactory instance, used to manage services, apps, roles, users, and platform configuration.
layout: schema
name: DreamFactory Admin
properties_list:
- description: Unique identifier for the administrator.
  name: id
  type: integer
- description: Display name of the administrator.
  name: name
  type: string
- description: First name of the administrator.
  name: first_name
  type: string
- description: Last name of the administrator.
  name: last_name
  type: string
- description: Email address used for login.
  name: email
  type: string
- description: Whether the admin account is active.
  name: is_active
  type: boolean
- description: Timestamp when the admin was created.
  name: created_date
  type: string
- description: Timestamp when the admin was last modified.
  name: last_modified_date
  type: string
provider_name: DreamFactory
provider_slug: dreamfactory
schema_file: json-schema/dreamfactory-admin.json
slug: dreamfactory-admin
source_filename: dreamfactory-admin.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-admin.json\",\n  \"title\": \"DreamFactory Admin\",\n  \"description\": \"A system administrator account in a DreamFactory instance, used to manage services, apps, roles, users, and platform configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the administrator.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the administrator.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the administrator.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the administrator.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"\
  email\",\n      \"description\": \"Email address used for login.\"\n    },\n    \"is_active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the admin account is active.\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the admin was created.\"\n    },\n    \"last_modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the admin was last modified.\"\n    }\n  },\n  \"required\": [\n    \"email\",\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-admin.json
tags:
- Automation
- Deployment
- Documentation
- Generation
- Security
title: DreamFactory Admin
---
