---
description: AddCustomRoutingEndpointsResponse schema from Amazon Global Accelerator API
layout: schema
name: AddCustomRoutingEndpointsResponse
properties_list:
- description: ''
  name: EndpointDescriptions
  type: object
- description: ''
  name: EndpointGroupArn
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-add-custom-routing-endpoints-response-schema.json
slug: global-accelerator-add-custom-routing-endpoints-response
source_filename: global-accelerator-add-custom-routing-endpoints-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-add-custom-routing-endpoints-response-schema.json\",\n  \"title\": \"AddCustomRoutingEndpointsResponse\",\n  \"description\": \"AddCustomRoutingEndpointsResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingEndpointDescriptions\"\n        },\n        {\n          \"description\": \"The endpoint objects added to the custom routing accelerator.\"\n        }\n      ]\n    },\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group for the custom routing\
  \ endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-add-custom-routing-endpoints-response-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: AddCustomRoutingEndpointsResponse
---
