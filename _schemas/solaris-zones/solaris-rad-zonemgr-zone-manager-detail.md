---
description: ZoneManager singleton providing system-wide zone management
layout: schema
name: ZoneManagerDetail
properties_list:
- description: Current evacuation state, null when no evacuation is active
  name: evacuationState
  type: '[''string'', ''null'']'
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-rad-zonemgr-zone-manager-detail-schema.json
slug: solaris-rad-zonemgr-zone-manager-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZoneManagerDetail\",\n  \"type\": \"object\",\n  \"description\": \"ZoneManager singleton providing system-wide zone management\",\n  \"properties\": {\n    \"evacuationState\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Current evacuation state, null when no evacuation is active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-rad-zonemgr-zone-manager-detail-schema.json
tags:
- Containers
- Kernel Zones
- Operating Systems
- Oracle
- RAD
- Resource Management
- Solaris
- StatsStore
- Virtualization
- Zones
title: ZoneManagerDetail
---
