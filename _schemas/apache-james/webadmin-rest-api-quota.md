---
description: Storage and message quota configuration
layout: schema
name: Quota
properties_list:
- description: Maximum number of messages (null for unlimited)
  name: count
  type: integer
- description: Maximum storage size in bytes (null for unlimited)
  name: size
  type: integer
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-quota-schema.json
slug: webadmin-rest-api-quota
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-quota-schema.json\",\n  \"title\": \"Quota\",\n  \"description\": \"Storage and message quota configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of messages (null for unlimited)\",\n      \"example\": 10000\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum storage size in bytes (null for unlimited)\",\n      \"example\": 1073741824\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-quota-schema.json
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: Quota
---
