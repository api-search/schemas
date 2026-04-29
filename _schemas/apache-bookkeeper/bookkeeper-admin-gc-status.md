---
description: Garbage collection status for a bookie.
layout: schema
name: GcStatus
properties_list:
- description: Whether forced garbage collection is currently active.
  name: is_in_force_gc
  type: string
provider_name: Apache BookKeeper
provider_slug: apache-bookkeeper
schema_file: json-schema/bookkeeper-admin-gc-status-schema.json
slug: bookkeeper-admin-gc-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-gc-status-schema.json\",\n  \"title\": \"GcStatus\",\n  \"description\": \"Garbage collection status for a bookie.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"is_in_force_gc\": { \"type\": \"string\", \"description\": \"Whether forced garbage collection is currently active.\", \"example\": \"false\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-gc-status-schema.json
tags:
- Apache
- Distributed Systems
- Log Storage
- Open Source
- Storage
- Streaming
title: GcStatus
---
