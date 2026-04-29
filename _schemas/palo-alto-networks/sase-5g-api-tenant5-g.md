---
description: Tenant5G schema from Palo Alto Networks SASE 5G Managed Services API
layout: schema
name: Tenant5G
properties_list:
- description: Unique identifier of the 5G tenant configuration.
  name: tenant_id
  type: string
- description: Tenant display name.
  name: name
  type: string
- description: Description of the tenant.
  name: description
  type: string
- description: Network slice IDs assigned to this tenant.
  name: assigned_slices
  type: array
- description: Default security policy ID for this tenant's traffic.
  name: default_policy_id
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-api-tenant5-g-schema.json
slug: sase-5g-api-tenant5-g
source_filename: sase-5g-api-tenant5-g-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tenant5G\",\n  \"description\": \"Tenant5G schema from Palo Alto Networks SASE 5G Managed Services API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-tenant5-g-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the 5G tenant configuration.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the tenant.\"\n    },\n    \"assigned_slices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Network slice IDs assigned to this tenant.\"\n    },\n    \"default_policy_id\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Default security policy ID for this tenant's traffic.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-tenant5-g-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Tenant5G
---
