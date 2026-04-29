---
description: CreateCustomRoutingEndpointGroupRequest schema from Amazon Global Accelerator API
layout: schema
name: CreateCustomRoutingEndpointGroupRequest
properties_list:
- description: ''
  name: ListenerArn
  type: object
- description: ''
  name: EndpointGroupRegion
  type: object
- description: ''
  name: DestinationConfigurations
  type: object
- description: ''
  name: IdempotencyToken
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-create-custom-routing-endpoint-group-request-schema.json
slug: global-accelerator-create-custom-routing-endpoint-group-request
source_filename: global-accelerator-create-custom-routing-endpoint-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-custom-routing-endpoint-group-request-schema.json\",\n  \"title\": \"CreateCustomRoutingEndpointGroupRequest\",\n  \"description\": \"CreateCustomRoutingEndpointGroupRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ListenerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the listener for a custom routing endpoint.\"\n        }\n      ]\n    },\n    \"EndpointGroupRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the endpoint group is located.\
  \ A listener can have only one endpoint group in a specific Region.\"\n        }\n      ]\n    },\n    \"DestinationConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingDestinationConfigurations\"\n        },\n        {\n          \"description\": \"Sets the port range and protocol for all endpoints (virtual private cloud subnets) in a custom routing endpoint group to accept client traffic on.\"\n        }\n      ]\n    },\n    \"IdempotencyToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive identifier that you provide to ensure the idempotency\\u2014that is, the uniqueness\\u2014of the request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ListenerArn\",\n    \"EndpointGroupRegion\",\n    \"DestinationConfigurations\",\n    \"IdempotencyToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-custom-routing-endpoint-group-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CreateCustomRoutingEndpointGroupRequest
---
