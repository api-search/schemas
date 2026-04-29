---
description: Shiro session information
layout: schema
name: Session
properties_list:
- description: Session identifier
  name: id
  type: string
- description: Session creation time
  name: startTimestamp
  type: string
- description: Last access time
  name: lastAccessTime
  type: string
- description: Session timeout in milliseconds
  name: timeout
  type: integer
- description: Host of the session initiator
  name: host
  type: string
- description: Whether the session has expired
  name: expired
  type: boolean
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-session-schema.json
slug: apache-shiro-session
source_filename: apache-shiro-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-session-schema.json\",\n  \"title\": \"Session\",\n  \"description\": \"Shiro session information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Session identifier\"\n    },\n    \"startTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Session creation time\"\n    },\n    \"lastAccessTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last access time\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Session timeout in milliseconds\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Host of the session initiator\"\n    },\n    \"\
  expired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the session has expired\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-session-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: Session
---
