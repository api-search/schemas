---
description: List of Knox topologies
layout: schema
name: TopologyList
properties_list:
- description: ''
  name: topologies
  type: object
provider_name: Apache Knox
provider_slug: apache-knox
schema_file: json-schema/admin-api-topology-list-schema.json
slug: admin-api-topology-list
source_filename: admin-api-topology-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-topology-list-schema.json\",\n  \"title\": \"TopologyList\",\n  \"description\": \"List of Knox topologies\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topologies\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"topology\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Topology\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-topology-list-schema.json
tags:
- API Gateway
- Authentication
- Hadoop
- Open Source
- Security
- SSO
title: TopologyList
---
