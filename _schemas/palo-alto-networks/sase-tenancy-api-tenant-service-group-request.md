---
description: TenantServiceGroupRequest schema from Palo Alto Networks SASE Tenancy Service API
layout: schema
name: TenantServiceGroupRequest
properties_list:
- description: Display name for the new TSG.
  name: display_name
  type: string
- description: Optional description of the TSG's purpose.
  name: description
  type: string
- description: ID of the parent TSG under which to create this TSG.
  name: parent_id
  type: string
- description: Palo Alto Networks support account ID to associate with this TSG.
  name: support_account_id
  type: string
- description: Industry vertical classification.
  name: vertical
  type: string
- description: Primary geographic region.
  name: region
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-tenancy-api-tenant-service-group-request-schema.json
slug: sase-tenancy-api-tenant-service-group-request
source_filename: sase-tenancy-api-tenant-service-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantServiceGroupRequest\",\n  \"description\": \"TenantServiceGroupRequest schema from Palo Alto Networks SASE Tenancy Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-tenancy-api-tenant-service-group-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the new TSG.\",\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the TSG's purpose.\",\n      \"maxLength\": 1024\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent TSG under which to create this TSG.\"\n    },\n    \"support_account_id\": {\n      \"type\": \"string\",\n      \"description\": \"Palo Alto Networks\
  \ support account ID to associate with this TSG.\"\n    },\n    \"vertical\": {\n      \"type\": \"string\",\n      \"description\": \"Industry vertical classification.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Primary geographic region.\"\n    }\n  },\n  \"required\": [\n    \"display_name\",\n    \"parent_id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-tenancy-api-tenant-service-group-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantServiceGroupRequest
---
