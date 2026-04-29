---
description: A zone configuration resource such as anet, fs, capped-cpu, etc.
layout: schema
name: Resource
properties_list:
- description: Resource type identifier
  name: type
  type: string
- description: List of properties for this resource
  name: properties
  type: array
- description: Parent resource reference for nested resources
  name: parent
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-rad-zonemgr-resource-schema.json
slug: solaris-rad-zonemgr-resource
source_filename: solaris-rad-zonemgr-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Resource\",\n  \"type\": \"object\",\n  \"description\": \"A zone configuration resource such as anet, fs, capped-cpu, etc.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"List of properties for this resource\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"Parent resource reference for nested resources\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-rad-zonemgr-resource-schema.json
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
