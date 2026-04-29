---
description: ''
layout: schema
name: GroupCreate
properties_list:
- description: Name for the new group.
  name: group
  type: string
- description: Configuration attributes for the group.
  name: group_attributes
  type: object
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-group-create-schema.json
slug: aruba-central-group-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new group.\"\n    },\n    \"group_attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration attributes for the group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-group-create-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: GroupCreate
---
