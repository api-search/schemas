---
description: Tenant5GRequest schema from Palo Alto Networks SASE 5G Managed Services API
layout: schema
name: Tenant5GRequest
properties_list:
- description: Display name for the tenant configuration.
  name: name
  type: string
- description: Optional description.
  name: description
  type: string
- description: Network slice IDs to assign to this tenant.
  name: assigned_slices
  type: array
- description: Default security policy ID for this tenant.
  name: default_policy_id
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-api-tenant5-g-request-schema.json
slug: sase-5g-api-tenant5-g-request
source_filename: sase-5g-api-tenant5-g-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tenant5GRequest\",\n  \"description\": \"Tenant5GRequest schema from Palo Alto Networks SASE 5G Managed Services API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-tenant5-g-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the tenant configuration.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description.\"\n    },\n    \"assigned_slices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Network slice IDs to assign to this tenant.\"\n    },\n    \"default_policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Default security policy ID for this tenant.\"\n    }\n  },\n  \"required\"\
  : [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-tenant5-g-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Tenant5GRequest
---
