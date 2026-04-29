---
description: ''
layout: schema
name: Property
properties_list:
- description: Property name
  name: name
  type: string
- description: Simple property value
  name: value
  type: string
- description: Property value type
  name: type
  type: string
- description: List of values for list-type properties
  name: listvalue
  type: array
- description: Complex property values
  name: complexvalue
  type: array
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-configuration-property-schema.json
slug: solaris-zone-configuration-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Property\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Property name\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Simple property value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Property value type\"\n    },\n    \"listvalue\": {\n      \"type\": \"array\",\n      \"description\": \"List of values for list-type properties\"\n    },\n    \"complexvalue\": {\n      \"type\": \"array\",\n      \"description\": \"Complex property values\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-configuration-property-schema.json
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
