---
description: A complex type for the endpoint group for a custom routing accelerator. An Amazon Web Services Region can have only one endpoint group for a specific listener.
layout: schema
name: CustomRoutingEndpointGroup
properties_list:
- description: ''
  name: EndpointGroupArn
  type: object
- description: ''
  name: EndpointGroupRegion
  type: object
- description: ''
  name: DestinationDescriptions
  type: object
- description: ''
  name: EndpointDescriptions
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-custom-routing-endpoint-group-schema.json
slug: global-accelerator-custom-routing-endpoint-group
source_filename: global-accelerator-custom-routing-endpoint-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-endpoint-group-schema.json\",\n  \"title\": \"CustomRoutingEndpointGroup\",\n  \"description\": \"A complex type for the endpoint group for a custom routing accelerator. An Amazon Web Services Region can have only one endpoint group for a specific listener. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group.\"\n        }\n      ]\n    },\n    \"EndpointGroupRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region\
  \ where the endpoint group is located.\"\n        }\n      ]\n    },\n    \"DestinationDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingDestinationDescriptions\"\n        },\n        {\n          \"description\": \"For a custom routing accelerator, describes the port range and protocol for all endpoints (virtual private cloud subnets) in an endpoint group to accept client traffic on.\"\n        }\n      ]\n    },\n    \"EndpointDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingEndpointDescriptions\"\n        },\n        {\n          \"description\": \"For a custom routing accelerator, describes the endpoints (virtual private cloud subnets) in an endpoint group to accept client traffic on.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-endpoint-group-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CustomRoutingEndpointGroup
---
