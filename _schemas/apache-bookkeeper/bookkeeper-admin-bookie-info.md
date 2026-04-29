---
description: Disk space information for a BookKeeper bookie.
layout: schema
name: BookieInfo
properties_list:
- description: Free disk space in bytes.
  name: freeSpace
  type: integer
- description: Total disk space in bytes.
  name: totalSpace
  type: integer
provider_name: Apache BookKeeper
provider_slug: apache-bookkeeper
schema_file: json-schema/bookkeeper-admin-bookie-info-schema.json
slug: bookkeeper-admin-bookie-info
source_filename: bookkeeper-admin-bookie-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-bookie-info-schema.json\",\n  \"title\": \"BookieInfo\",\n  \"description\": \"Disk space information for a BookKeeper bookie.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"freeSpace\": { \"type\": \"integer\", \"format\": \"int64\", \"description\": \"Free disk space in bytes.\", \"example\": 107374182400 },\n    \"totalSpace\": { \"type\": \"integer\", \"format\": \"int64\", \"description\": \"Total disk space in bytes.\", \"example\": 214748364800 }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-bookie-info-schema.json
tags:
- Apache
- Distributed Systems
- Log Storage
- Open Source
- Storage
- Streaming
title: BookieInfo
---
