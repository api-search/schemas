---
description: SortBy schema from Multi-Tenant Notifications API
layout: schema
name: SortBy
properties_list:
- description: Sort field
  name: field
  type: string
- description: Ascending or Descending
  name: sortBy
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-sort-by-schema.json
slug: sase-multitenant-notifications-api-sort-by
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SortBy\",\n  \"description\": \"SortBy schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-sort-by-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"description\": \"Sort field\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"createdTime\",\n        \"impactedTenantCount\"\n      ]\n    },\n    \"sortBy\": {\n      \"description\": \"Ascending or Descending\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"DESC\",\n        \"ASC\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-sort-by-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SortBy
---
