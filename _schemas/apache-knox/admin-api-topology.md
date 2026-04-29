---
description: A Knox gateway topology
layout: schema
name: Topology
properties_list:
- description: Topology name
  name: name
  type: string
- description: Topology gateway URL
  name: uri
  type: string
- description: Last modified timestamp
  name: timestamp
  type: integer
provider_name: Apache Knox
provider_slug: apache-knox
schema_file: json-schema/admin-api-topology-schema.json
slug: admin-api-topology
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-topology-schema.json\",\n  \"title\": \"Topology\",\n  \"description\": \"A Knox gateway topology\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Topology name\",\n      \"example\": \"sandbox\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"Topology gateway URL\",\n      \"example\": \"https://localhost:8443/gateway/sandbox\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Last modified timestamp\",\n      \"example\": 1718153645993\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-topology-schema.json
tags:
- API Gateway
- Authentication
- Hadoop
- Open Source
- Security
- SSO
title: Topology
---
