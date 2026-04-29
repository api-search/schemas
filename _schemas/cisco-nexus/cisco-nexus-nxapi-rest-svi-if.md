---
description: Switch Virtual Interface managed object for Layer 3 VLAN routing. DN format is sys/intf/svi-[{id}].
layout: schema
name: SviIf
properties_list:
- description: ''
  name: attributes
  type: object
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
schema_file: json-schema/cisco-nexus-nxapi-rest-svi-if-schema.json
slug: cisco-nexus-nxapi-rest-svi-if
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SviIf\",\n  \"type\": \"object\",\n  \"description\": \"Switch Virtual Interface managed object for Layer 3 VLAN routing. DN format is sys/intf/svi-[{id}].\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/json-schema/cisco-nexus-nxapi-rest-svi-if-schema.json
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
title: SviIf
---
