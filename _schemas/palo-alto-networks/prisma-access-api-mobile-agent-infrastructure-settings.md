---
description: MobileAgentInfrastructureSettings schema from Palo Alto Networks Prisma Access Configuration API
layout: schema
name: MobileAgentInfrastructureSettings
properties_list:
- description: ''
  name: id
  type: string
- description: Name for the infrastructure settings configuration.
  name: name
  type: string
- description: IP address pools for mobile user address allocation.
  name: ip_pool
  type: array
- description: DNS server IP addresses for mobile users.
  name: dns_servers
  type: array
- description: DNS suffixes to append for mobile users.
  name: dns_suffix
  type: array
- description: Compute regions for mobile user connectivity.
  name: regions
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-api-mobile-agent-infrastructure-settings-schema.json
slug: prisma-access-api-mobile-agent-infrastructure-settings
source_filename: prisma-access-api-mobile-agent-infrastructure-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MobileAgentInfrastructureSettings\",\n  \"description\": \"MobileAgentInfrastructureSettings schema from Palo Alto Networks Prisma Access Configuration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-mobile-agent-infrastructure-settings-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the infrastructure settings configuration.\"\n    },\n    \"ip_pool\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IP address pools for mobile user address allocation.\"\n    },\n    \"dns_servers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n\
  \      \"description\": \"DNS server IP addresses for mobile users.\"\n    },\n    \"dns_suffix\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"DNS suffixes to append for mobile users.\"\n    },\n    \"regions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Prisma Access compute region.\"\n          },\n          \"addresses\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"IP addresses for the mobile user gateway in this region.\"\n          }\n        }\n      },\n      \"description\": \"Compute regions for mobile user connectivity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-mobile-agent-infrastructure-settings-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MobileAgentInfrastructureSettings
---
