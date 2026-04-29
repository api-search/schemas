---
description: Defender schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: Defender
properties_list:
- description: Hostname where the Defender is deployed.
  name: hostname
  type: string
- description: Defender agent version.
  name: version
  type: string
- description: Type of Defender deployment.
  name: type
  type: string
- description: Whether the Defender is currently connected to the Console.
  name: connected
  type: boolean
- description: Timestamp of the last status update from the Defender.
  name: lastModified
  type: string
- description: Kubernetes cluster name if applicable.
  name: cluster
  type: string
- description: ''
  name: cloudMetadata
  type: object
- description: ''
  name: category
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-defender-schema.json
slug: prisma-cloud-compute-api-defender
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Defender\",\n  \"description\": \"Defender schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-defender-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname where the Defender is deployed.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Defender agent version.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"docker\",\n        \"dockerWindows\",\n        \"cri\",\n        \"fargate\",\n        \"appEmbedded\",\n        \"serverless\"\n      ],\n      \"description\": \"Type of Defender deployment.\"\n    },\n    \"connected\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the Defender is currently connected to the Console.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last status update from the Defender.\"\n    },\n    \"cluster\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes cluster name if applicable.\"\n    },\n    \"cloudMetadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"provider\": {\n          \"type\": \"string\"\n        },\n        \"accountId\": {\n          \"type\": \"string\"\n        },\n        \"region\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"container\",\n        \"host\",\n        \"serverless\",\n        \"appEmbedded\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-defender-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Defender
---
