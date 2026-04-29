---
description: CreateCustomRoutingEndpointGroupResponse schema from Amazon Global Accelerator API
layout: schema
name: CreateCustomRoutingEndpointGroupResponse
properties_list:
- description: ''
  name: EndpointGroup
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-create-custom-routing-endpoint-group-response-schema.json
slug: global-accelerator-create-custom-routing-endpoint-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-custom-routing-endpoint-group-response-schema.json\",\n  \"title\": \"CreateCustomRoutingEndpointGroupResponse\",\n  \"description\": \"CreateCustomRoutingEndpointGroupResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingEndpointGroup\"\n        },\n        {\n          \"description\": \"The information about the endpoint group created for a custom routing accelerator.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-custom-routing-endpoint-group-response-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CreateCustomRoutingEndpointGroupResponse
---
