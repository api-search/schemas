---
description: Layer 2 bridge domain managed object representing a VLAN. DN format is sys/bd/bd-[{fabEncap}].
layout: schema
name: L2BD
properties_list:
- description: ''
  name: attributes
  type: object
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
schema_file: json-schema/cisco-nexus-nxapi-rest-l2-bd-schema.json
slug: cisco-nexus-nxapi-rest-l2-bd
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"L2BD\",\n  \"type\": \"object\",\n  \"description\": \"Layer 2 bridge domain managed object representing a VLAN. DN format is sys/bd/bd-[{fabEncap}].\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/json-schema/cisco-nexus-nxapi-rest-l2-bd-schema.json
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
title: L2BD
---
