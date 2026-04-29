---
description: A mail repository for storing messages
layout: schema
name: MailRepository
properties_list:
- description: Repository path
  name: repository
  type: string
- description: Repository identifier
  name: id
  type: string
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-mail-repository-schema.json
slug: webadmin-rest-api-mail-repository
source_filename: webadmin-rest-api-mail-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-mail-repository-schema.json\",\n  \"title\": \"MailRepository\",\n  \"description\": \"A mail repository for storing messages\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repository\": {\n      \"type\": \"string\",\n      \"description\": \"Repository path\",\n      \"example\": \"var/mail/error/\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Repository identifier\",\n      \"example\": \"var%2Fmail%2Ferror%2F\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-mail-repository-schema.json
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: MailRepository
---
