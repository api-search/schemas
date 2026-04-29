---
description: MappingRequest schema from SASE 5G Monitor Service API
layout: schema
name: MappingRequest
properties_list:
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: pageNum
  type: integer
- description: ''
  name: searchKey
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: tenant
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-monitor-api-mapping-request-schema.json
slug: sase-5g-monitor-api-mapping-request
source_filename: sase-5g-monitor-api-mapping-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MappingRequest\",\n  \"description\": \"MappingRequest schema from SASE 5G Monitor Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-monitor-api-mapping-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"pageNum\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"searchKey\": {\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"tenant\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-monitor-api-mapping-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MappingRequest
---
