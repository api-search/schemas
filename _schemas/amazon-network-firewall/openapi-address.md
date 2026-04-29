---
description: A single IP address specification. This is used in the <a>MatchAttributes</a> source and destination specifications.
layout: schema
name: Address
properties_list:
- description: ''
  name: AddressDefinition
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-address-schema.json
slug: openapi-address
source_filename: openapi-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"A single IP address specification. This is used in the <a>MatchAttributes</a> source and destination specifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AddressDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressDefinition\"\n        },\n        {\n          \"description\": \"<p>Specify an IP address or a block of IP addresses in Classless Inter-Domain Routing (CIDR) notation. Network Firewall supports all address ranges for IPv4 and IPv6. </p> <p>Examples: </p> <ul> <li> <p>To configure Network Firewall to inspect for the IP address 192.0.2.44, specify <code>192.0.2.44/32</code>.</p> </li> <li> <p>To configure Network Firewall to inspect for IP addresses\
  \ from 192.0.2.0 to 192.0.2.255, specify <code>192.0.2.0/24</code>.</p> </li> <li> <p>To configure Network Firewall to inspect for the IP address 1111:0000:0000:0000:0000:0000:0000:0111, specify <code>1111:0000:0000:0000:0000:0000:0000:0111/128</code>.</p> </li> <li> <p>To configure Network Firewall to inspect for IP addresses from 1111:0000:0000:0000:0000:0000:0000:0000 to 1111:0000:0000:0000:ffff:ffff:ffff:ffff, specify <code>1111:0000:0000:0000:0000:0000:0000:0000/64</code>.</p> </li> </ul> <p>For more information about CIDR notation, see the Wikipedia entry <a href=\\\"https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing\\\">Classless Inter-Domain Routing</a>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AddressDefinition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-address-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: Address
---
