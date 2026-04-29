---
description: A complex type for the set of IP addresses for an accelerator.
layout: schema
name: IpSet
properties_list:
- description: ''
  name: IpFamily
  type: object
- description: ''
  name: IpAddresses
  type: object
- description: ''
  name: IpAddressFamily
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-ip-set-schema.json
slug: global-accelerator-ip-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-ip-set-schema.json\",\n  \"title\": \"IpSet\",\n  \"description\": \"A complex type for the set of IP addresses for an accelerator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpFamily\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"IpFamily is deprecated and has been replaced by IpAddressFamily.IpFamily has been replaced by IpAddressFamily\"\n        }\n      ]\n    },\n    \"IpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddresses\"\n        },\n        {\n          \"description\": \"The array of IP addresses in the IP address set. An IP address set can have a maximum of two IP addresses.\"\
  \n        }\n      ]\n    },\n    \"IpAddressFamily\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressFamily\"\n        },\n        {\n          \"description\": \"The types of IP addresses included in this IP set. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-ip-set-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: IpSet
---
