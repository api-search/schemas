---
description: Top-level BGP entity managed object. DN is sys/bgp.
layout: schema
name: BgpEntity
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: children
  type: array
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
schema_file: json-schema/cisco-nexus-nxapi-rest-bgp-entity-schema.json
slug: cisco-nexus-nxapi-rest-bgp-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BgpEntity\",\n  \"type\": \"object\",\n  \"description\": \"Top-level BGP entity managed object. DN is sys/bgp.\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\"\n    },\n    \"children\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/json-schema/cisco-nexus-nxapi-rest-bgp-entity-schema.json
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
title: BgpEntity
---
