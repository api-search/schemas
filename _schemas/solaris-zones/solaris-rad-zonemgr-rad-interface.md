---
description: A RAD interface entry describing an available management object
layout: schema
name: RadInterface
properties_list:
- description: Relative URI to the interface
  name: href
  type: string
- description: Interface type name
  name: type
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-rad-zonemgr-rad-interface-schema.json
slug: solaris-rad-zonemgr-rad-interface
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RadInterface\",\n  \"type\": \"object\",\n  \"description\": \"A RAD interface entry describing an available management object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URI to the interface\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Interface type name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-rad-zonemgr-rad-interface-schema.json
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
title: RadInterface
---
