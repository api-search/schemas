---
description: TenantSummary schema from Palo Alto Networks SASE Aggregate Monitoring API
layout: schema
name: TenantSummary
properties_list:
- description: Tenant Service Group ID.
  name: tsg_id
  type: string
- description: TSG display name.
  name: display_name
  type: string
- description: Parent TSG ID.
  name: parent_id
  type: string
- description: Depth in the hierarchy (0 for root).
  name: depth
  type: integer
- description: Number of direct child TSGs.
  name: child_count
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-aggregate-monitoring-api-tenant-summary-schema.json
slug: sase-aggregate-monitoring-api-tenant-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantSummary\",\n  \"description\": \"TenantSummary schema from Palo Alto Networks SASE Aggregate Monitoring API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-aggregate-monitoring-api-tenant-summary-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service Group ID.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"TSG display name.\"\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"description\": \"Parent TSG ID.\"\n    },\n    \"depth\": {\n      \"type\": \"integer\",\n      \"description\": \"Depth in the hierarchy (0 for root).\"\n    },\n    \"child_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of direct child TSGs.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-aggregate-monitoring-api-tenant-summary-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantSummary
---
