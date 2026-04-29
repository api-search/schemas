---
description: BGP instance managed object containing AS number and domain configuration. DN is sys/bgp/inst.
layout: schema
name: BgpInst
properties_list:
- description: ''
  name: bgpInst
  type: object
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
schema_file: json-schema/cisco-nexus-nxapi-rest-bgp-inst-schema.json
slug: cisco-nexus-nxapi-rest-bgp-inst
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BgpInst\",\n  \"type\": \"object\",\n  \"description\": \"BGP instance managed object containing AS number and domain configuration. DN is sys/bgp/inst.\",\n  \"properties\": {\n    \"bgpInst\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/json-schema/cisco-nexus-nxapi-rest-bgp-inst-schema.json
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
title: BgpInst
---
