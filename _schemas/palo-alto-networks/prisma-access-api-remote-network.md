---
description: RemoteNetwork schema from Palo Alto Networks Prisma Access Configuration API
layout: schema
name: RemoteNetwork
properties_list:
- description: Unique identifier for the remote network.
  name: id
  type: string
- description: Name of the remote network.
  name: name
  type: string
- description: Prisma Access compute region (e.g., us-east-1, eu-west-1).
  name: region
  type: string
- description: License type assigned to this remote network.
  name: license_type
  type: string
- description: Service provider node name for the Prisma Access gateway location.
  name: spn_name
  type: string
- description: Enable or disable ECMP load balancing.
  name: ecmp_load_balancing
  type: string
- description: Local subnets at the remote network site.
  name: subnets
  type: array
- description: Folder containing this remote network.
  name: folder
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-api-remote-network-schema.json
slug: prisma-access-api-remote-network
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RemoteNetwork\",\n  \"description\": \"RemoteNetwork schema from Palo Alto Networks Prisma Access Configuration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-remote-network-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the remote network.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the remote network.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Prisma Access compute region (e.g., us-east-1, eu-west-1).\"\n    },\n    \"license_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"FWAAS-AGGREGATE\",\n        \"FWAAS-BYOL\"\n      ],\n      \"description\": \"License type assigned\
  \ to this remote network.\"\n    },\n    \"spn_name\": {\n      \"type\": \"string\",\n      \"description\": \"Service provider node name for the Prisma Access gateway location.\"\n    },\n    \"ecmp_load_balancing\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"enable\",\n        \"disable\"\n      ],\n      \"description\": \"Enable or disable ECMP load balancing.\"\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Local subnets at the remote network site.\"\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"description\": \"Folder containing this remote network.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"region\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-remote-network-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RemoteNetwork
---
