---
description: UpdateCustomRoutingListenerRequest schema from Amazon Global Accelerator API
layout: schema
name: UpdateCustomRoutingListenerRequest
properties_list:
- description: ''
  name: ListenerArn
  type: object
- description: ''
  name: PortRanges
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-update-custom-routing-listener-request-schema.json
slug: global-accelerator-update-custom-routing-listener-request
source_filename: global-accelerator-update-custom-routing-listener-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-custom-routing-listener-request-schema.json\",\n  \"title\": \"UpdateCustomRoutingListenerRequest\",\n  \"description\": \"UpdateCustomRoutingListenerRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ListenerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the listener to update.\"\n        }\n      ]\n    },\n    \"PortRanges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRanges\"\n        },\n        {\n          \"description\": \"<p>The updated port range to support for connections from clients to your accelerator. If you remove ports that\
  \ are currently being used by a subnet endpoint, the call fails.</p> <p>Separately, you set port ranges for endpoints. For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/about-custom-routing-endpoints.html\\\">About endpoints for custom routing accelerators</a>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ListenerArn\",\n    \"PortRanges\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-custom-routing-listener-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UpdateCustomRoutingListenerRequest
---
