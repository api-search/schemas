---
description: Criteria for Network Firewall to use to inspect an individual packet in stateless rule inspection. Each match attributes set can include one or more items such as IP address, CIDR range, port number, protocol, and TCP flags.
layout: schema
name: MatchAttributes
properties_list:
- description: ''
  name: Sources
  type: object
- description: ''
  name: Destinations
  type: object
- description: ''
  name: SourcePorts
  type: object
- description: ''
  name: DestinationPorts
  type: object
- description: ''
  name: Protocols
  type: object
- description: ''
  name: TCPFlags
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-match-attributes-schema.json
slug: openapi-match-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-match-attributes-schema.json\",\n  \"title\": \"MatchAttributes\",\n  \"description\": \"Criteria for Network Firewall to use to inspect an individual packet in stateless rule inspection. Each match attributes set can include one or more items such as IP address, CIDR range, port number, protocol, and TCP flags. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Addresses\"\n        },\n        {\n          \"description\": \"The source IP addresses and address ranges to inspect for, in CIDR notation. If not specified, this matches with any source address. \"\n        }\n      ]\n    },\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Addresses\"\
  \n        },\n        {\n          \"description\": \"The destination IP addresses and address ranges to inspect for, in CIDR notation. If not specified, this matches with any destination address. \"\n        }\n      ]\n    },\n    \"SourcePorts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRanges\"\n        },\n        {\n          \"description\": \"<p>The source ports to inspect for. If not specified, this matches with any source port. This setting is only used for protocols 6 (TCP) and 17 (UDP). </p> <p>You can specify individual ports, for example <code>1994</code> and you can specify port ranges, for example <code>1990:1994</code>. </p>\"\n        }\n      ]\n    },\n    \"DestinationPorts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRanges\"\n        },\n        {\n          \"description\": \"<p>The destination ports to inspect for. If not specified, this matches with any destination port. This setting\
  \ is only used for protocols 6 (TCP) and 17 (UDP). </p> <p>You can specify individual ports, for example <code>1994</code> and you can specify port ranges, for example <code>1990:1994</code>. </p>\"\n        }\n      ]\n    },\n    \"Protocols\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtocolNumbers\"\n        },\n        {\n          \"description\": \"The protocols to inspect for, specified using each protocol's assigned internet protocol number (IANA). If not specified, this matches with any protocol. \"\n        }\n      ]\n    },\n    \"TCPFlags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TCPFlags\"\n        },\n        {\n          \"description\": \"The TCP flags and masks to inspect for. If not specified, this matches with any settings. This setting is only used for protocol 6 (TCP).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-match-attributes-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: MatchAttributes
---
