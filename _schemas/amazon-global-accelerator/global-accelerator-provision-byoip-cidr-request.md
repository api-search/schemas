---
description: ProvisionByoipCidrRequest schema from Amazon Global Accelerator API
layout: schema
name: ProvisionByoipCidrRequest
properties_list:
- description: ''
  name: Cidr
  type: object
- description: ''
  name: CidrAuthorizationContext
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-provision-byoip-cidr-request-schema.json
slug: global-accelerator-provision-byoip-cidr-request
source_filename: global-accelerator-provision-byoip-cidr-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-provision-byoip-cidr-request-schema.json\",\n  \"title\": \"ProvisionByoipCidrRequest\",\n  \"description\": \"ProvisionByoipCidrRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cidr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The public IPv4 address range, in CIDR notation. The most specific IP prefix that you can specify is /24. The address range cannot overlap with another address range that you've brought to this or another Region.\"\n        }\n      ]\n    },\n    \"CidrAuthorizationContext\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CidrAuthorizationContext\"\n        },\n\
  \        {\n          \"description\": \"A signed document that proves that you are authorized to bring the specified IP address range to Amazon using BYOIP. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Cidr\",\n    \"CidrAuthorizationContext\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-provision-byoip-cidr-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: ProvisionByoipCidrRequest
---
