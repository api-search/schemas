---
description: A virtual system (vsys) on the PAN-OS firewall.
layout: schema
name: VirtualSystem
properties_list:
- description: Virtual system name (e.g., vsys1, vsys2).
  name: '@name'
  type: string
- description: Human-readable display name for the vsys.
  name: display-name
  type: string
- description: Imported network resources for this vsys.
  name: import
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-virtual-system-schema.json
slug: pan-os-rest-api-virtual-system
source_filename: pan-os-rest-api-virtual-system-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VirtualSystem\",\n  \"description\": \"A virtual system (vsys) on the PAN-OS firewall.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-virtual-system-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@name\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual system name (e.g., vsys1, vsys2).\"\n    },\n    \"display-name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the vsys.\"\n    },\n    \"import\": {\n      \"type\": \"object\",\n      \"description\": \"Imported network resources for this vsys.\",\n      \"properties\": {\n        \"network\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"interface\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"member\"\
  : {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  },\n                  \"description\": \"Network interfaces assigned to this vsys.\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-virtual-system-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: VirtualSystem
---
