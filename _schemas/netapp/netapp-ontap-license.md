---
description: Cluster feature license
layout: schema
name: License
properties_list:
- description: License name
  name: name
  type: string
- description: License scope
  name: scope
  type: string
- description: License compliance state
  name: state
  type: string
- description: Individual license entries
  name: licenses
  type: array
provider_name: NetApp
provider_slug: netapp
schema_file: json-schema/netapp-ontap-license-schema.json
slug: netapp-ontap-license
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"License\",\n  \"type\": \"object\",\n  \"description\": \"Cluster feature license\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"License name\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"License scope\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"License compliance state\"\n    },\n    \"licenses\": {\n      \"type\": \"array\",\n      \"description\": \"Individual license entries\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/json-schema/netapp-ontap-license-schema.json
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
title: License
---
