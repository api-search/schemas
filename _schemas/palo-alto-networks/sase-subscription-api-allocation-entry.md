---
description: AllocationEntry schema from Palo Alto Networks SASE Subscription Service API
layout: schema
name: AllocationEntry
properties_list:
- description: Child TSG ID receiving this allocation.
  name: tsg_id
  type: string
- description: Display name of the child TSG.
  name: tsg_name
  type: string
- description: Quantity allocated to this TSG.
  name: allocated_quantity
  type: integer
- description: Quantity currently utilized by this TSG.
  name: utilized_quantity
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-subscription-api-allocation-entry-schema.json
slug: sase-subscription-api-allocation-entry
source_filename: sase-subscription-api-allocation-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AllocationEntry\",\n  \"description\": \"AllocationEntry schema from Palo Alto Networks SASE Subscription Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-allocation-entry-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Child TSG ID receiving this allocation.\"\n    },\n    \"tsg_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the child TSG.\"\n    },\n    \"allocated_quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity allocated to this TSG.\"\n    },\n    \"utilized_quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity currently utilized by this TSG.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-allocation-entry-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AllocationEntry
---
