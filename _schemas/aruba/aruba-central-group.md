---
description: Configuration group for organizing devices and applying shared configuration templates, firmware policies, and settings.
layout: schema
name: Group
properties_list:
- description: Name of the group.
  name: group
  type: string
- description: Group-level configuration properties.
  name: group_properties
  type: object
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-group-schema.json
slug: aruba-central-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"type\": \"object\",\n  \"description\": \"Configuration group for organizing devices and applying shared configuration templates, firmware policies, and settings.\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the group.\"\n    },\n    \"group_properties\": {\n      \"type\": \"object\",\n      \"description\": \"Group-level configuration properties.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-group-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: Group
---
