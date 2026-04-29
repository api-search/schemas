---
description: Disk group schema from Veritas InfoScale REST API
layout: schema
name: DiskGroup
properties_list:
- description: Disk group name
  name: name
  type: string
- description: Disk group state
  name: state
  type: string
- description: Total disk group size
  name: totalSize
  type: string
- description: Free space in disk group
  name: freeSize
  type: string
- description: Number of disks in the group
  name: diskCount
  type: integer
- description: Number of volumes in the group
  name: volumeCount
  type: integer
- description: Default layout type
  name: layout
  type: string
- description: Disk group version
  name: version
  type: string
provider_name: Veritas InfoScale
provider_slug: veritas-infoscale
schema_file: json-schema/rest-api-disk-group-schema.json
slug: rest-api-disk-group
source_filename: rest-api-disk-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-disk-group-schema.json\",\n  \"title\": \"DiskGroup\",\n  \"description\": \"Disk group schema from Veritas InfoScale REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Disk group name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"enabled\", \"disabled\", \"deported\"],\n      \"description\": \"Disk group state\"\n    },\n    \"totalSize\": {\n      \"type\": \"string\",\n      \"description\": \"Total disk group size\"\n    },\n    \"freeSize\": {\n      \"type\": \"string\",\n      \"description\": \"Free space in disk group\"\n    },\n    \"diskCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of disks in the group\"\n    },\n    \"volumeCount\": {\n     \
  \ \"type\": \"integer\",\n      \"description\": \"Number of volumes in the group\"\n    },\n    \"layout\": {\n      \"type\": \"string\",\n      \"enum\": [\"concat\", \"stripe\", \"mirror\", \"raid5\"],\n      \"description\": \"Default layout type\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Disk group version\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-disk-group-schema.json
tags:
- Clustering
- Data Management
- Disaster Recovery
- High Availability
- Storage Management
- Virtualization
title: DiskGroup
---
