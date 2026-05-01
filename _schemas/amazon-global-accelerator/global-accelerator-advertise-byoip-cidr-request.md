---
description: AdvertiseByoipCidrRequest schema from Amazon Global Accelerator API
layout: schema
name: AdvertiseByoipCidrRequest
properties_list:
- description: ''
  name: Cidr
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-advertise-byoip-cidr-request-schema.json
slug: global-accelerator-advertise-byoip-cidr-request
source_filename: global-accelerator-advertise-byoip-cidr-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-advertise-byoip-cidr-request-schema.json\",\n  \"title\": \"AdvertiseByoipCidrRequest\",\n  \"description\": \"AdvertiseByoipCidrRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cidr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The address range, in CIDR notation. This must be the exact range that you provisioned. You can't advertise only a portion of the provisioned range.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Cidr\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-advertise-byoip-cidr-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: AdvertiseByoipCidrRequest
---
