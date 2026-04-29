---
description: A node in the QueryGrid environment.
layout: schema
name: Node
properties_list:
- description: Unique node identifier.
  name: id
  type: string
- description: Node name.
  name: name
  type: string
- description: Node hostname.
  name: hostname
  type: string
- description: Parent system identifier.
  name: systemId
  type: string
- description: Node status.
  name: status
  type: string
- description: Installed software version.
  name: softwareVersion
  type: string
provider_name: Teradata
provider_slug: teradata
schema_file: json-schema/querygrid-manager-api-node-schema.json
slug: querygrid-manager-api-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-node-schema.json\",\n  \"title\": \"Node\",\n  \"description\": \"A node in the QueryGrid environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique node identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Node name.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Node hostname.\"\n    },\n    \"systemId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent system identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Node status.\",\n      \"enum\": [\"active\", \"inactive\", \"error\"]\n    },\n    \"softwareVersion\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Installed software version.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-node-schema.json
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
title: Node
---
