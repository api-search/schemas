---
description: Represents a configurable resource within an Oracle Solaris Zone, such as a network interface, device, filesystem, resource control, or CPU/memory allocation. Resources are managed through the zonecfg interface exposed via the RAD zonemgr module.
layout: schema
name: Oracle Solaris Zone Resource
properties_list:
- description: Resource type identifier determining the kind of resource
  name: type
  type: string
- description: Array of property name-value pairs for the resource
  name: properties
  type: array
- description: Reference to a parent resource, if applicable
  name: parent
  type:
  - string
  - 'null'
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-resource-schema.json
slug: solaris-zone-resource
source_filename: solaris-zone-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/solaris/zone-resource.json\",\n  \"title\": \"Oracle Solaris Zone Resource\",\n  \"description\": \"Represents a configurable resource within an Oracle Solaris Zone, such as a network interface, device, filesystem, resource control, or CPU/memory allocation. Resources are managed through the zonecfg interface exposed via the RAD zonemgr module.\",\n  \"type\": \"object\",\n  \"required\": [\"type\"],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier determining the kind of resource\",\n      \"enum\": [\n        \"net\",\n        \"anet\",\n        \"device\",\n        \"fs\",\n        \"dataset\",\n        \"rctl\",\n        \"attr\",\n        \"dedicated-cpu\",\n        \"capped-memory\",\n        \"capped-cpu\",\n        \"admin\",\n        \"security-flags\",\n        \"suspend\"\n      ]\n\
  \    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Property\"\n      },\n      \"description\": \"Array of property name-value pairs for the resource\"\n    },\n    \"parent\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Reference to a parent resource, if applicable\"\n    }\n  },\n  \"$defs\": {\n    \"Property\": {\n      \"type\": \"object\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Property name (e.g., physical, address, dir, special, ncpus, physical, locked)\"\n        },\n        \"value\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Simple scalar property value\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Property value type classification\",\n          \"enum\": [\"simple\", \"list\", \"complex\"],\n          \"default\"\
  : \"simple\"\n        },\n        \"listvalue\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Array of values for list-type properties\"\n        },\n        \"complexvalue\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Array of values for complex-type properties (key=value pairs)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-resource-schema.json
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
title: Oracle Solaris Zone Resource
---
