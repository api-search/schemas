---
description: Service group schema from Veritas InfoScale REST API
layout: schema
name: ServiceGroup
properties_list:
- description: Service group name
  name: name
  type: string
- description: Current service group state
  name: state
  type: string
- description: List of systems where this group can run
  name: systemList
  type: array
- description: System where the group is currently online
  name: currentSystem
  type: string
- description: Whether the group starts automatically
  name: autoStart
  type: boolean
- description: Whether the group can run on multiple systems
  name: parallel
  type: boolean
- description: Number of resources in this group
  name: resourceCount
  type: integer
- description: Type classification of the service group
  name: groupType
  type: string
- description: Whether this is a critical service group
  name: critical
  type: boolean
provider_name: Veritas InfoScale
provider_slug: veritas-infoscale
schema_file: json-schema/rest-api-service-group-schema.json
slug: rest-api-service-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-service-group-schema.json\",\n  \"title\": \"ServiceGroup\",\n  \"description\": \"Service group schema from Veritas InfoScale REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Service group name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"ONLINE\", \"OFFLINE\", \"FAULTED\", \"PARTIAL\", \"STARTING\", \"STOPPING\"],\n      \"description\": \"Current service group state\"\n    },\n    \"systemList\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"List of systems where this group can run\"\n    },\n    \"currentSystem\": {\n      \"type\": \"string\",\n      \"description\": \"System where the group is currently online\"\n    },\n\
  \    \"autoStart\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the group starts automatically\"\n    },\n    \"parallel\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the group can run on multiple systems\"\n    },\n    \"resourceCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of resources in this group\"\n    },\n    \"groupType\": {\n      \"type\": \"string\",\n      \"description\": \"Type classification of the service group\"\n    },\n    \"critical\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a critical service group\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-service-group-schema.json
tags:
- Clustering
- Data Management
- Disaster Recovery
- High Availability
- Storage Management
- Virtualization
title: ServiceGroup
---
