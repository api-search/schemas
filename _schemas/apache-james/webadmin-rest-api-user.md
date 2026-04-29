---
description: A James mail server user account
layout: schema
name: User
properties_list:
- description: User email address
  name: username
  type: string
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-user-schema.json
slug: webadmin-rest-api-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"A James mail server user account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"User email address\",\n      \"example\": \"user@example.com\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-user-schema.json
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: User
---
