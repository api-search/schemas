---
description: ''
layout: schema
name: Property
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: value
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: listvalue
  type: array
- description: ''
  name: complexvalue
  type: array
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-unified-archives-property-schema.json
slug: solaris-unified-archives-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Property\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"listvalue\": {\n      \"type\": \"array\"\n    },\n    \"complexvalue\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-unified-archives-property-schema.json
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
title: Property
---
