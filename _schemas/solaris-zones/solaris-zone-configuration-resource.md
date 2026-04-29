---
description: ''
layout: schema
name: Resource
properties_list:
- description: 'Resource type name. Common types include: net, anet, device, fs, dataset, rctl, attr, dedicated-cpu, capped-memory, capped-cpu, admin, security-flags'
  name: type
  type: string
- description: Resource properties
  name: properties
  type: array
- description: Parent resource reference
  name: parent
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-configuration-resource-schema.json
slug: solaris-zone-configuration-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type name. Common types include: net, anet, device, fs, dataset, rctl, attr, dedicated-cpu, capped-memory, capped-cpu, admin, security-flags\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Resource properties\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"Parent resource reference\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-configuration-resource-schema.json
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
title: Resource
---
