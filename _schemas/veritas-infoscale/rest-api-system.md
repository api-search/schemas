---
description: Cluster system node schema from Veritas InfoScale REST API
layout: schema
name: System
properties_list:
- description: System hostname
  name: name
  type: string
- description: System state in the cluster
  name: state
  type: string
- description: Whether the system is frozen
  name: frozen
  type: boolean
- description: Current CPU usage percentage
  name: cpuUsage
  type: number
- description: Current memory usage percentage
  name: memoryUsage
  type: number
- description: Number of service groups on this system
  name: serviceGroupCount
  type: integer
- description: Operating system platform
  name: platform
  type: string
- description: Hardware architecture
  name: architecture
  type: string
provider_name: Veritas InfoScale
provider_slug: veritas-infoscale
schema_file: json-schema/rest-api-system-schema.json
slug: rest-api-system
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-system-schema.json\",\n  \"title\": \"System\",\n  \"description\": \"Cluster system node schema from Veritas InfoScale REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"System hostname\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"RUNNING\", \"FAULTED\", \"EXITED\", \"UNKNOWN\"],\n      \"description\": \"System state in the cluster\"\n    },\n    \"frozen\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the system is frozen\"\n    },\n    \"cpuUsage\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Current CPU usage percentage\"\n    },\n    \"memoryUsage\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n\
  \      \"description\": \"Current memory usage percentage\"\n    },\n    \"serviceGroupCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of service groups on this system\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system platform\"\n    },\n    \"architecture\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware architecture\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-system-schema.json
tags:
- Clustering
- Data Management
- Disaster Recovery
- High Availability
- Storage Management
- Virtualization
title: System
---
