---
description: Represents an Oracle Solaris Zone instance managed through the RAD zonemgr module, including its identity, brand type, lifecycle state, and auxiliary state information.
layout: schema
name: Oracle Solaris Zone
properties_list:
- description: Unique zone name used as the primary identifier
  name: name
  type: string
- description: Zone brand type determining the virtualization model
  name: brand
  type: string
- description: Numeric zone ID assigned when the zone is running or ready. The global zone is always ID 0.
  name: id
  type: integer
- description: Universally unique identifier for the zone
  name: uuid
  type:
  - string
  - 'null'
- description: Current lifecycle state of the zone
  name: state
  type: string
- description: Dynamic auxiliary state flags providing additional status information
  name: auxstate
  type: array
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-schema.json
slug: solaris-zone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/solaris/zone.json\",\n  \"title\": \"Oracle Solaris Zone\",\n  \"description\": \"Represents an Oracle Solaris Zone instance managed through the RAD zonemgr module, including its identity, brand type, lifecycle state, and auxiliary state information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique zone name used as the primary identifier\",\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9._-]*$\",\n      \"maxLength\": 64\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Zone brand type determining the virtualization model\",\n      \"enum\": [\"solaris\", \"solaris-kz\", \"solaris10\", \"labeled\"],\n      \"examples\": [\"solaris\", \"solaris-kz\"]\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric zone ID assigned when the\
  \ zone is running or ready. The global zone is always ID 0.\",\n      \"minimum\": -1\n    },\n    \"uuid\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uuid\",\n      \"description\": \"Universally unique identifier for the zone\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle state of the zone\",\n      \"enum\": [\n        \"configured\",\n        \"incomplete\",\n        \"installed\",\n        \"ready\",\n        \"running\",\n        \"shutting_down\",\n        \"down\"\n      ]\n    },\n    \"auxstate\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Dynamic auxiliary state flags providing additional status information\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-schema.json
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
title: Oracle Solaris Zone
---
