---
description: The list of endpoint objects. For custom routing, this is a list of virtual private cloud (VPC) subnet IDs.
layout: schema
name: CustomRoutingEndpointConfiguration
properties_list:
- description: ''
  name: EndpointId
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-custom-routing-endpoint-configuration-schema.json
slug: global-accelerator-custom-routing-endpoint-configuration
source_filename: global-accelerator-custom-routing-endpoint-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-endpoint-configuration-schema.json\",\n  \"title\": \"CustomRoutingEndpointConfiguration\",\n  \"description\": \"The list of endpoint objects. For custom routing, this is a list of virtual private cloud (VPC) subnet IDs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"An ID for the endpoint. For custom routing accelerators, this is the virtual private cloud (VPC) subnet ID. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-endpoint-configuration-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CustomRoutingEndpointConfiguration
---
