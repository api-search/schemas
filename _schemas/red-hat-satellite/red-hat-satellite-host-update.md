---
description: Parameters for updating an existing host.
layout: schema
name: HostUpdate
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: ip
  type: string
- description: ''
  name: mac
  type: string
- description: ''
  name: architecture_id
  type: integer
- description: ''
  name: domain_id
  type: integer
- description: ''
  name: subnet_id
  type: integer
- description: ''
  name: operatingsystem_id
  type: integer
- description: ''
  name: hostgroup_id
  type: integer
- description: ''
  name: location_id
  type: integer
- description: ''
  name: organization_id
  type: integer
- description: ''
  name: owner_id
  type: integer
- description: ''
  name: owner_type
  type: string
- description: ''
  name: build
  type: boolean
- description: ''
  name: managed
  type: boolean
- description: ''
  name: comment
  type: string
- description: ''
  name: content_facet_attributes
  type: object
- description: ''
  name: interfaces_attributes
  type: array
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-host-update-schema.json
slug: red-hat-satellite-host-update
source_filename: red-hat-satellite-host-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HostUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Parameters for updating an existing host.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"ip\": {\n      \"type\": \"string\"\n    },\n    \"mac\": {\n      \"type\": \"string\"\n    },\n    \"architecture_id\": {\n      \"type\": \"integer\"\n    },\n    \"domain_id\": {\n      \"type\": \"integer\"\n    },\n    \"subnet_id\": {\n      \"type\": \"integer\"\n    },\n    \"operatingsystem_id\": {\n      \"type\": \"integer\"\n    },\n    \"hostgroup_id\": {\n      \"type\": \"integer\"\n    },\n    \"location_id\": {\n      \"type\": \"integer\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\"\n    },\n    \"owner_id\": {\n      \"type\": \"integer\"\n    },\n    \"owner_type\": {\n      \"type\": \"string\"\n    },\n    \"build\": {\n      \"type\": \"boolean\"\n    },\n    \"managed\"\
  : {\n      \"type\": \"boolean\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    },\n    \"content_facet_attributes\": {\n      \"type\": \"object\"\n    },\n    \"interfaces_attributes\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-host-update-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: HostUpdate
---
