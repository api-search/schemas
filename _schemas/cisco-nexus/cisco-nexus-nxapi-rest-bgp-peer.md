---
description: BGP peer (neighbor) managed object. DN format is sys/bgp/inst/dom-{name}/peer-{addr}.
layout: schema
name: BgpPeer
properties_list:
- description: ''
  name: bgpPeer
  type: object
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
schema_file: json-schema/cisco-nexus-nxapi-rest-bgp-peer-schema.json
slug: cisco-nexus-nxapi-rest-bgp-peer
source_filename: cisco-nexus-nxapi-rest-bgp-peer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BgpPeer\",\n  \"type\": \"object\",\n  \"description\": \"BGP peer (neighbor) managed object. DN format is sys/bgp/inst/dom-{name}/peer-{addr}.\",\n  \"properties\": {\n    \"bgpPeer\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/json-schema/cisco-nexus-nxapi-rest-bgp-peer-schema.json
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
title: BgpPeer
---
