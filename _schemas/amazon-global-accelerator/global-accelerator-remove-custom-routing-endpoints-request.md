---
description: RemoveCustomRoutingEndpointsRequest schema from Amazon Global Accelerator API
layout: schema
name: RemoveCustomRoutingEndpointsRequest
properties_list:
- description: ''
  name: EndpointIds
  type: object
- description: ''
  name: EndpointGroupArn
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-remove-custom-routing-endpoints-request-schema.json
slug: global-accelerator-remove-custom-routing-endpoints-request
source_filename: global-accelerator-remove-custom-routing-endpoints-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-remove-custom-routing-endpoints-request-schema.json\",\n  \"title\": \"RemoveCustomRoutingEndpointsRequest\",\n  \"description\": \"RemoveCustomRoutingEndpointsRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointIds\"\n        },\n        {\n          \"description\": \"The IDs for the endpoints. For custom routing accelerators, endpoint IDs are the virtual private cloud (VPC) subnet IDs. \"\n        }\n      ]\n    },\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of\
  \ the endpoint group to remove endpoints from.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointIds\",\n    \"EndpointGroupArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-remove-custom-routing-endpoints-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: RemoveCustomRoutingEndpointsRequest
---
