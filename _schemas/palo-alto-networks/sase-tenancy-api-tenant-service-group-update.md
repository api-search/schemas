---
description: TenantServiceGroupUpdate schema from Palo Alto Networks SASE Tenancy Service API
layout: schema
name: TenantServiceGroupUpdate
properties_list:
- description: New display name for the TSG.
  name: display_name
  type: string
- description: Updated description.
  name: description
  type: string
- description: Updated industry vertical classification.
  name: vertical
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-tenancy-api-tenant-service-group-update-schema.json
slug: sase-tenancy-api-tenant-service-group-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantServiceGroupUpdate\",\n  \"description\": \"TenantServiceGroupUpdate schema from Palo Alto Networks SASE Tenancy Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-tenancy-api-tenant-service-group-update-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"New display name for the TSG.\",\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Updated description.\",\n      \"maxLength\": 1024\n    },\n    \"vertical\": {\n      \"type\": \"string\",\n      \"description\": \"Updated industry vertical classification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-tenancy-api-tenant-service-group-update-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantServiceGroupUpdate
---
