---
description: BGP domain (VRF) managed object. DN format is sys/bgp/inst/dom-{name}.
layout: schema
name: BgpDom
properties_list:
- description: ''
  name: bgpDom
  type: object
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
schema_file: json-schema/cisco-nexus-nxapi-rest-bgp-dom-schema.json
slug: cisco-nexus-nxapi-rest-bgp-dom
source_filename: cisco-nexus-nxapi-rest-bgp-dom-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BgpDom\",\n  \"type\": \"object\",\n  \"description\": \"BGP domain (VRF) managed object. DN format is sys/bgp/inst/dom-{name}.\",\n  \"properties\": {\n    \"bgpDom\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/json-schema/cisco-nexus-nxapi-rest-bgp-dom-schema.json
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
title: BgpDom
---
