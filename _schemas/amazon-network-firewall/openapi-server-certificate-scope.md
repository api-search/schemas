---
description: Settings that define the Secure Sockets Layer/Transport Layer Security (SSL/TLS) traffic that Network Firewall should decrypt for inspection by the stateful rule engine.
layout: schema
name: ServerCertificateScope
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
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-server-certificate-scope-schema.json
slug: openapi-server-certificate-scope
source_filename: openapi-server-certificate-scope-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-server-certificate-scope-schema.json\",\n  \"title\": \"ServerCertificateScope\",\n  \"description\": \"Settings that define the Secure Sockets Layer/Transport Layer Security (SSL/TLS) traffic that Network Firewall should decrypt for inspection by the stateful rule engine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Addresses\"\n        },\n        {\n          \"description\": \"The source IP addresses and address ranges to decrypt for inspection, in CIDR notation. If not specified, this matches with any source address.\"\n        }\n      ]\n    },\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Addresses\"\n        },\n        {\n   \
  \       \"description\": \"The destination IP addresses and address ranges to decrypt for inspection, in CIDR notation. If not specified, this matches with any destination address.\"\n        }\n      ]\n    },\n    \"SourcePorts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRanges\"\n        },\n        {\n          \"description\": \"<p>The source ports to decrypt for inspection, in Transmission Control Protocol (TCP) format. If not specified, this matches with any source port.</p> <p>You can specify individual ports, for example <code>1994</code>, and you can specify port ranges, such as <code>1990:1994</code>.</p>\"\n        }\n      ]\n    },\n    \"DestinationPorts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRanges\"\n        },\n        {\n          \"description\": \"<p>The destination ports to decrypt for inspection, in Transmission Control Protocol (TCP) format. If not specified, this matches with any\
  \ destination port.</p> <p>You can specify individual ports, for example <code>1994</code>, and you can specify port ranges, such as <code>1990:1994</code>.</p>\"\n        }\n      ]\n    },\n    \"Protocols\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtocolNumbers\"\n        },\n        {\n          \"description\": \"The protocols to decrypt for inspection, specified using each protocol's assigned internet protocol number (IANA). Network Firewall currently supports only TCP.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-server-certificate-scope-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: ServerCertificateScope
---
