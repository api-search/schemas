---
description: Information about the currently elected auditor bookie.
layout: schema
name: AuditorInfo
properties_list:
- description: Hostname and address of the elected auditor.
  name: Auditor
  type: string
provider_name: Apache BookKeeper
provider_slug: apache-bookkeeper
schema_file: json-schema/bookkeeper-admin-auditor-info-schema.json
slug: bookkeeper-admin-auditor-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-auditor-info-schema.json\",\n  \"title\": \"AuditorInfo\",\n  \"description\": \"Information about the currently elected auditor bookie.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Auditor\": { \"type\": \"string\", \"description\": \"Hostname and address of the elected auditor.\", \"example\": \"bookie1.example.com/192.168.1.1:3181\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-bookkeeper/refs/heads/main/json-schema/bookkeeper-admin-auditor-info-schema.json
tags:
- Apache
- Distributed Systems
- Log Storage
- Open Source
- Storage
- Streaming
title: AuditorInfo
---
