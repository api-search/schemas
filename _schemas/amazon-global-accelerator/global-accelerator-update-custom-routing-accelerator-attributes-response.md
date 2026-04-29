---
description: UpdateCustomRoutingAcceleratorAttributesResponse schema from Amazon Global Accelerator API
layout: schema
name: UpdateCustomRoutingAcceleratorAttributesResponse
properties_list:
- description: ''
  name: AcceleratorAttributes
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-update-custom-routing-accelerator-attributes-response-schema.json
slug: global-accelerator-update-custom-routing-accelerator-attributes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-custom-routing-accelerator-attributes-response-schema.json\",\n  \"title\": \"UpdateCustomRoutingAcceleratorAttributesResponse\",\n  \"description\": \"UpdateCustomRoutingAcceleratorAttributesResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingAcceleratorAttributes\"\n        },\n        {\n          \"description\": \"Updated custom routing accelerator.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-custom-routing-accelerator-attributes-response-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UpdateCustomRoutingAcceleratorAttributesResponse
---
