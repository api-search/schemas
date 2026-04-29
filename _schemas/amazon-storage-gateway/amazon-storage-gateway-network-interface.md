---
description: Describes a gateway's network interface.
layout: schema
name: NetworkInterface
properties_list:
- description: ''
  name: Ipv4Address
  type: object
- description: ''
  name: MacAddress
  type: object
- description: ''
  name: Ipv6Address
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-network-interface-schema.json
slug: amazon-storage-gateway-network-interface
source_filename: amazon-storage-gateway-network-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-network-interface-schema.json\",\n  \"title\": \"NetworkInterface\",\n  \"description\": \"Describes a gateway's network interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Ipv4Address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The Internet Protocol version 4 (IPv4) address of the interface.\"\n        }\n      ]\n    },\n    \"MacAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"<p>The Media Access Control (MAC) address of the interface.</p> <note> <p>This is currently unsupported and will not be returned in output.</p> </note>\"\n        }\n      ]\n    },\n  \
  \  \"Ipv6Address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The Internet Protocol version 6 (IPv6) address of the interface. <i>Currently not supported</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-network-interface-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: NetworkInterface
---
