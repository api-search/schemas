---
description: Information about the client application used in an event.
layout: schema
name: EventClient
properties_list:
- description: The name of the 1Password application.
  name: app_name
  type: string
- description: The version of the application.
  name: app_version
  type: string
- description: The name of the operating system platform.
  name: platform_name
  type: string
- description: The version of the operating system.
  name: platform_version
  type: string
- description: The name of the operating system.
  name: os_name
  type: string
- description: The version of the operating system.
  name: os_version
  type: string
- description: The IP address of the client.
  name: ip
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-events-event-client-schema.json
slug: 1password-events-event-client
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-event-client-schema.json\",\n  \"title\": \"EventClient\",\n  \"description\": \"Information about the client application used in an event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the 1Password application.\"\n    },\n    \"app_version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the application.\"\n    },\n    \"platform_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the operating system platform.\"\n    },\n    \"platform_version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the operating system.\"\n    },\n    \"os_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the operating system.\"\
  \n    },\n    \"os_version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the operating system.\"\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address of the client.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-event-client-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: EventClient
---
