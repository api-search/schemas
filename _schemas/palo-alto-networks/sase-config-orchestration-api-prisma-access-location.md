---
description: PrismaAccessLocation schema from Palo Alto Networks SASE Configuration Orchestration API
layout: schema
name: PrismaAccessLocation
properties_list:
- description: Location identifier used in API requests.
  name: name
  type: string
- description: Human-readable location name.
  name: display_name
  type: string
- description: Geographic region (e.g., americas, europe, asia-pacific).
  name: region
  type: string
- description: Country code (ISO 3166-1 alpha-2).
  name: country
  type: string
- description: City name.
  name: city
  type: string
- description: Current availability status.
  name: status
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-config-orchestration-api-prisma-access-location-schema.json
slug: sase-config-orchestration-api-prisma-access-location
source_filename: sase-config-orchestration-api-prisma-access-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PrismaAccessLocation\",\n  \"description\": \"PrismaAccessLocation schema from Palo Alto Networks SASE Configuration Orchestration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-prisma-access-location-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Location identifier used in API requests.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable location name.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic region (e.g., americas, europe, asia-pacific).\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code (ISO 3166-1 alpha-2).\"\n    },\n    \"city\": {\n      \"type\": \"\
  string\",\n      \"description\": \"City name.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"available\",\n        \"limited\",\n        \"unavailable\"\n      ],\n      \"description\": \"Current availability status.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-prisma-access-location-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PrismaAccessLocation
---
