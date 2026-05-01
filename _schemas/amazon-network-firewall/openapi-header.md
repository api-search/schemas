---
description: The basic rule criteria for Network Firewall to use to inspect packet headers in stateful traffic flow inspection. Traffic flows that match the criteria are a match for the corresponding <a>StatefulRule</a>.
layout: schema
name: Header
properties_list:
- description: ''
  name: Protocol
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: SourcePort
  type: object
- description: ''
  name: Direction
  type: object
- description: ''
  name: Destination
  type: object
- description: ''
  name: DestinationPort
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-header-schema.json
slug: openapi-header
source_filename: openapi-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-header-schema.json\",\n  \"title\": \"Header\",\n  \"description\": \"The basic rule criteria for Network Firewall to use to inspect packet headers in stateful traffic flow inspection. Traffic flows that match the criteria are a match for the corresponding <a>StatefulRule</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatefulRuleProtocol\"\n        },\n        {\n          \"description\": \"The protocol to inspect for. To specify all, you can use <code>IP</code>, because all traffic on Amazon Web Services and on the internet is IP.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Source\"\n        },\n      \
  \  {\n          \"description\": \"<p>The source IP address or address range to inspect for, in CIDR notation. To match with any address, specify <code>ANY</code>. </p> <p>Specify an IP address or a block of IP addresses in Classless Inter-Domain Routing (CIDR) notation. Network Firewall supports all address ranges for IPv4 and IPv6. </p> <p>Examples: </p> <ul> <li> <p>To configure Network Firewall to inspect for the IP address 192.0.2.44, specify <code>192.0.2.44/32</code>.</p> </li> <li> <p>To configure Network Firewall to inspect for IP addresses from 192.0.2.0 to 192.0.2.255, specify <code>192.0.2.0/24</code>.</p> </li> <li> <p>To configure Network Firewall to inspect for the IP address 1111:0000:0000:0000:0000:0000:0000:0111, specify <code>1111:0000:0000:0000:0000:0000:0000:0111/128</code>.</p> </li> <li> <p>To configure Network Firewall to inspect for IP addresses from 1111:0000:0000:0000:0000:0000:0000:0000 to 1111:0000:0000:0000:ffff:ffff:ffff:ffff, specify <code>1111:0000:0000:0000:0000:0000:0000:0000/64</code>.</p>\
  \ </li> </ul> <p>For more information about CIDR notation, see the Wikipedia entry <a href=\\\"https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing\\\">Classless Inter-Domain Routing</a>.</p>\"\n        }\n      ]\n    },\n    \"SourcePort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Port\"\n        },\n        {\n          \"description\": \"The source port to inspect for. You can specify an individual port, for example <code>1994</code> and you can specify a port range, for example <code>1990:1994</code>. To match with any port, specify <code>ANY</code>. \"\n        }\n      ]\n    },\n    \"Direction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatefulRuleDirection\"\n        },\n        {\n          \"description\": \"The direction of traffic flow to inspect. If set to <code>ANY</code>, the inspection matches bidirectional traffic, both from the source to the destination and from the destination to the source.\
  \ If set to <code>FORWARD</code>, the inspection only matches traffic going from the source to the destination. \"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Destination\"\n        },\n        {\n          \"description\": \"<p>The destination IP address or address range to inspect for, in CIDR notation. To match with any address, specify <code>ANY</code>. </p> <p>Specify an IP address or a block of IP addresses in Classless Inter-Domain Routing (CIDR) notation. Network Firewall supports all address ranges for IPv4 and IPv6. </p> <p>Examples: </p> <ul> <li> <p>To configure Network Firewall to inspect for the IP address 192.0.2.44, specify <code>192.0.2.44/32</code>.</p> </li> <li> <p>To configure Network Firewall to inspect for IP addresses from 192.0.2.0 to 192.0.2.255, specify <code>192.0.2.0/24</code>.</p> </li> <li> <p>To configure Network Firewall to inspect for the IP address 1111:0000:0000:0000:0000:0000:0000:0111,\
  \ specify <code>1111:0000:0000:0000:0000:0000:0000:0111/128</code>.</p> </li> <li> <p>To configure Network Firewall to inspect for IP addresses from 1111:0000:0000:0000:0000:0000:0000:0000 to 1111:0000:0000:0000:ffff:ffff:ffff:ffff, specify <code>1111:0000:0000:0000:0000:0000:0000:0000/64</code>.</p> </li> </ul> <p>For more information about CIDR notation, see the Wikipedia entry <a href=\\\"https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing\\\">Classless Inter-Domain Routing</a>.</p>\"\n        }\n      ]\n    },\n    \"DestinationPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Port\"\n        },\n        {\n          \"description\": \"The destination port to inspect for. You can specify an individual port, for example <code>1994</code> and you can specify a port range, for example <code>1990:1994</code>. To match with any port, specify <code>ANY</code>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Protocol\",\n    \"Source\"\
  ,\n    \"SourcePort\",\n    \"Direction\",\n    \"Destination\",\n    \"DestinationPort\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-header-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: Header
---
