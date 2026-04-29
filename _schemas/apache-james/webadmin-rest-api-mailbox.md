---
description: A user mailbox
layout: schema
name: Mailbox
properties_list:
- description: Mailbox folder name
  name: mailboxName
  type: string
- description: Unique mailbox identifier
  name: mailboxId
  type: string
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-mailbox-schema.json
slug: webadmin-rest-api-mailbox
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-mailbox-schema.json\",\n  \"title\": \"Mailbox\",\n  \"description\": \"A user mailbox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mailboxName\": {\n      \"type\": \"string\",\n      \"description\": \"Mailbox folder name\",\n      \"example\": \"INBOX\"\n    },\n    \"mailboxId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique mailbox identifier\",\n      \"example\": \"mailbox-1234\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-mailbox-schema.json
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: Mailbox
---
