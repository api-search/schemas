---
description: ''
layout: schema
name: KernelZoneResource
properties_list:
- description: Resource type. Kernel zone specific types include dedicated-cpu and capped-memory for virtual hardware allocation.
  name: type
  type: string
- description: Resource property values
  name: properties
  type: array
- description: Parent resource reference
  name: parent
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-kernel-zones-kernel-zone-resource-schema.json
slug: solaris-kernel-zones-kernel-zone-resource
source_filename: solaris-kernel-zones-kernel-zone-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KernelZoneResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type. Kernel zone specific types include dedicated-cpu and capped-memory for virtual hardware allocation.\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Resource property values\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"Parent resource reference\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-kernel-zones-kernel-zone-resource-schema.json
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
title: KernelZoneResource
---
