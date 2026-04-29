---
description: BandwidthAllocation schema from Palo Alto Networks SASE Configuration Orchestration API
layout: schema
name: BandwidthAllocation
properties_list:
- description: Prisma Access location name.
  name: location
  type: string
- description: Geographic region.
  name: region
  type: string
- description: Total licensed bandwidth at this location in Mbps.
  name: licensed_bandwidth_mbps
  type: integer
- description: Bandwidth currently allocated to remote networks in Mbps.
  name: allocated_bandwidth_mbps
  type: integer
- description: Remaining available bandwidth in Mbps.
  name: available_bandwidth_mbps
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-config-orchestration-api-bandwidth-allocation-schema.json
slug: sase-config-orchestration-api-bandwidth-allocation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BandwidthAllocation\",\n  \"description\": \"BandwidthAllocation schema from Palo Alto Networks SASE Configuration Orchestration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-bandwidth-allocation-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Prisma Access location name.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic region.\"\n    },\n    \"licensed_bandwidth_mbps\": {\n      \"type\": \"integer\",\n      \"description\": \"Total licensed bandwidth at this location in Mbps.\"\n    },\n    \"allocated_bandwidth_mbps\": {\n      \"type\": \"integer\",\n      \"description\": \"Bandwidth currently allocated to remote networks in Mbps.\"\n    },\n    \"available_bandwidth_mbps\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Remaining available bandwidth in Mbps.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-bandwidth-allocation-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BandwidthAllocation
---
