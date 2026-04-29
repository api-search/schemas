---
description: Helix cluster instance (participant) configuration
layout: schema
name: Instance
properties_list:
- description: Instance name
  name: id
  type: string
- description: Hostname of the instance
  name: hostName
  type: string
- description: Port number
  name: port
  type: integer
- description: Whether the instance is enabled
  name: enabled
  type: boolean
- description: Instance tags
  name: tags
  type: array
provider_name: Apache Helix
provider_slug: apache-helix
schema_file: json-schema/helix-rest-instance-schema.json
slug: helix-rest-instance
source_filename: helix-rest-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-helix/json-schema/helix-rest-instance-schema.json\",\n  \"title\": \"Instance\",\n  \"type\": \"object\",\n  \"description\": \"Helix cluster instance (participant) configuration\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Instance name\",\n      \"example\": \"localhost_12913\"\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the instance\",\n      \"example\": \"localhost\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number\",\n      \"example\": 12913\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the instance is enabled\",\n      \"example\": true\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\"\
  : \"Instance tags\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-helix/refs/heads/main/json-schema/helix-rest-instance-schema.json
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: Instance
---
