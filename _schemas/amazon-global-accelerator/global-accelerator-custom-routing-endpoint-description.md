---
description: A complex type for an endpoint for a custom routing accelerator. Each endpoint group can include one or more endpoints, which are virtual private cloud (VPC) subnets.
layout: schema
name: CustomRoutingEndpointDescription
properties_list:
- description: ''
  name: EndpointId
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-custom-routing-endpoint-description-schema.json
slug: global-accelerator-custom-routing-endpoint-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-endpoint-description-schema.json\",\n  \"title\": \"CustomRoutingEndpointDescription\",\n  \"description\": \"A complex type for an endpoint for a custom routing accelerator. Each endpoint group can include one or more endpoints, which are virtual private cloud (VPC) subnets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"An ID for the endpoint. For custom routing accelerators, this is the virtual private cloud (VPC) subnet ID. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-endpoint-description-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CustomRoutingEndpointDescription
---
