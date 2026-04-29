---
description: A datastore within the Cobalt embedded integration platform for managing structured records.
layout: schema
name: Datastore
properties_list:
- description: Datastore ID.
  name: _id
  type: string
- description: Datastore name.
  name: name
  type: string
- description: Datastore slug.
  name: slug
  type: string
- description: Associated configuration ID.
  name: config_id
  type: string
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/datastore.json
slug: datastore
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/datastore.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Datastore\",\n  \"description\": \"A datastore within the Cobalt embedded integration platform for managing structured records.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Datastore ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Datastore name.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"Datastore slug.\"\n    },\n    \"config_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated configuration ID.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/datastore.json
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Datastore
---
