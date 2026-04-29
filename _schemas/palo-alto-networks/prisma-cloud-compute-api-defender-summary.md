---
description: DefenderSummary schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: DefenderSummary
properties_list:
- description: Total number of deployed Defenders.
  name: total
  type: integer
- description: Number of currently connected Defenders.
  name: connected
  type: integer
- description: Number of disconnected Defenders.
  name: disconnected
  type: integer
- description: Defender count breakdown by deployment type.
  name: by_type
  type: object
- description: ''
  name: version_distribution
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-defender-summary-schema.json
slug: prisma-cloud-compute-api-defender-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DefenderSummary\",\n  \"description\": \"DefenderSummary schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-defender-summary-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of deployed Defenders.\"\n    },\n    \"connected\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of currently connected Defenders.\"\n    },\n    \"disconnected\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of disconnected Defenders.\"\n    },\n    \"by_type\": {\n      \"type\": \"object\",\n      \"description\": \"Defender count breakdown by deployment type.\",\n      \"properties\": {\n        \"docker\": {\n          \"type\": \"integer\"\
  \n        },\n        \"dockerWindows\": {\n          \"type\": \"integer\"\n        },\n        \"cri\": {\n          \"type\": \"integer\"\n        },\n        \"fargate\": {\n          \"type\": \"integer\"\n        },\n        \"appEmbedded\": {\n          \"type\": \"integer\"\n        },\n        \"serverless\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"version_distribution\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"version\": {\n            \"type\": \"string\"\n          },\n          \"count\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-defender-summary-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DefenderSummary
---
