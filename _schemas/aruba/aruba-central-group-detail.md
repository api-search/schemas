---
description: ''
layout: schema
name: GroupDetail
properties_list:
- description: Name of the group.
  name: group
  type: string
- description: ''
  name: group_properties
  type: object
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-group-detail-schema.json
slug: aruba-central-group-detail
source_filename: aruba-central-group-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the group.\"\n    },\n    \"group_properties\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-group-detail-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: GroupDetail
---
