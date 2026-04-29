---
description: A zone resource property with support for simple, list, and complex values
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
  name: listValue
  type: array
- description: Complex structured values
  name: complexValue
  type: array
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-rad-zonemgr-property-schema.json
slug: solaris-rad-zonemgr-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Property\",\n  \"type\": \"object\",\n  \"description\": \"A zone resource property with support for simple, list, and complex values\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Property name\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Simple property value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Property value type\"\n    },\n    \"listValue\": {\n      \"type\": \"array\",\n      \"description\": \"List of values for list-type properties\"\n    },\n    \"complexValue\": {\n      \"type\": \"array\",\n      \"description\": \"Complex structured values\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-rad-zonemgr-property-schema.json
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
