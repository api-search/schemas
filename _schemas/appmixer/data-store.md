---
description: A Data Store is a key-value storage mechanism in Appmixer that allows flows to persist and share data across executions.
layout: schema
name: Appmixer Data Store
properties_list:
- description: Unique identifier for the data store.
  name: storeId
  type: string
- description: Human-readable name of the data store.
  name: name
  type: string
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/data-store.json
slug: data-store
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/appmixer/blob/main/json-schema/data-store.json\",\n  \"title\": \"Appmixer Data Store\",\n  \"description\": \"A Data Store is a key-value storage mechanism in Appmixer that allows flows to persist and share data across executions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"storeId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the data store.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the data store.\"\n    }\n  },\n  \"required\": [\"storeId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/json-schema/data-store.json
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer Data Store
---
