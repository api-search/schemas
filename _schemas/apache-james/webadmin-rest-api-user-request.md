---
description: Request body for user creation
layout: schema
name: UserRequest
properties_list:
- description: User email address
  name: username
  type: string
- description: User password
  name: password
  type: string
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-user-request-schema.json
slug: webadmin-rest-api-user-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-user-request-schema.json\",\n  \"title\": \"UserRequest\",\n  \"description\": \"Request body for user creation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"User email address\",\n      \"example\": \"user@example.com\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"User password\",\n      \"example\": \"securepassword\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-user-request-schema.json
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: UserRequest
---
