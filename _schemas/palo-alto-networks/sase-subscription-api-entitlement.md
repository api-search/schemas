---
description: Entitlement schema from Palo Alto Networks SASE Subscription Service API
layout: schema
name: Entitlement
properties_list:
- description: Feature or capability name.
  name: feature
  type: string
- description: Licensed quantity for this entitlement.
  name: licensed_quantity
  type: integer
- description: Quantity already allocated to child TSGs.
  name: allocated_quantity
  type: integer
- description: Remaining quantity available for allocation.
  name: available_quantity
  type: integer
- description: Unit of measure.
  name: unit
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-subscription-api-entitlement-schema.json
slug: sase-subscription-api-entitlement
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Entitlement\",\n  \"description\": \"Entitlement schema from Palo Alto Networks SASE Subscription Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-entitlement-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"feature\": {\n      \"type\": \"string\",\n      \"description\": \"Feature or capability name.\"\n    },\n    \"licensed_quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Licensed quantity for this entitlement.\"\n    },\n    \"allocated_quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity already allocated to child TSGs.\"\n    },\n    \"available_quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Remaining quantity available for allocation.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Unit of measure.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-entitlement-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Entitlement
---
