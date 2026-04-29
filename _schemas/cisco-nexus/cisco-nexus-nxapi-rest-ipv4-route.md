---
description: IPv4 static route managed object. DN format is sys/ipv4/inst/dom-{vrfName}/rt-[{prefix}].
layout: schema
name: Ipv4Route
properties_list:
- description: ''
  name: attributes
  type: object
- description: Child next-hop objects
  name: children
  type: array
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
schema_file: json-schema/cisco-nexus-nxapi-rest-ipv4-route-schema.json
slug: cisco-nexus-nxapi-rest-ipv4-route
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Ipv4Route\",\n  \"type\": \"object\",\n  \"description\": \"IPv4 static route managed object. DN format is sys/ipv4/inst/dom-{vrfName}/rt-[{prefix}].\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\"\n    },\n    \"children\": {\n      \"type\": \"array\",\n      \"description\": \"Child next-hop objects\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/json-schema/cisco-nexus-nxapi-rest-ipv4-route-schema.json
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
title: Ipv4Route
---
