---
description: IPv4 next-hop specification for a static route. DN format is sys/ipv4/inst/dom-{vrfName}/rt-[{prefix}]/nh-[{nhIf}]-addr-[{nhAddr}]-vrf-[{nhVrf}].
layout: schema
name: Ipv4Nexthop
properties_list:
- description: ''
  name: ipv4Nexthop
  type: object
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
schema_file: json-schema/cisco-nexus-nxapi-rest-ipv4-nexthop-schema.json
slug: cisco-nexus-nxapi-rest-ipv4-nexthop
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Ipv4Nexthop\",\n  \"type\": \"object\",\n  \"description\": \"IPv4 next-hop specification for a static route. DN format is sys/ipv4/inst/dom-{vrfName}/rt-[{prefix}]/nh-[{nhIf}]-addr-[{nhAddr}]-vrf-[{nhVrf}].\",\n  \"properties\": {\n    \"ipv4Nexthop\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/json-schema/cisco-nexus-nxapi-rest-ipv4-nexthop-schema.json
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
title: Ipv4Nexthop
---
