---
description: ''
layout: schema
name: KstatInterface
properties_list:
- description: URL path to the kstat interface
  name: href
  type: string
- description: Kstat module name
  name: module
  type: string
- description: Kstat name
  name: name
  type: string
- description: Statistic name
  name: statistic
  type: string
- description: Instance identifier
  name: instance
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-monitoring-kstat-interface-schema.json
slug: solaris-zone-monitoring-kstat-interface
source_filename: solaris-zone-monitoring-kstat-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KstatInterface\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"URL path to the kstat interface\"\n    },\n    \"module\": {\n      \"type\": \"string\",\n      \"description\": \"Kstat module name\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Kstat name\"\n    },\n    \"statistic\": {\n      \"type\": \"string\",\n      \"description\": \"Statistic name\"\n    },\n    \"instance\": {\n      \"type\": \"string\",\n      \"description\": \"Instance identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-monitoring-kstat-interface-schema.json
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
title: KstatInterface
---
