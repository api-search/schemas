---
description: For a custom routing accelerator, sets the port range and protocol for all endpoints (virtual private cloud subnets) in an endpoint group to accept client traffic on.
layout: schema
name: CustomRoutingDestinationConfiguration
properties_list:
- description: ''
  name: FromPort
  type: object
- description: ''
  name: ToPort
  type: object
- description: ''
  name: Protocols
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-custom-routing-destination-configuration-schema.json
slug: global-accelerator-custom-routing-destination-configuration
source_filename: global-accelerator-custom-routing-destination-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-destination-configuration-schema.json\",\n  \"title\": \"CustomRoutingDestinationConfiguration\",\n  \"description\": \"For a custom routing accelerator, sets the port range and protocol for all endpoints (virtual private cloud subnets) in an endpoint group to accept client traffic on.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FromPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The first port, inclusive, in the range of ports for the endpoint group that is associated with a custom routing accelerator.\"\n        }\n      ]\n    },\n    \"ToPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n      \
  \  },\n        {\n          \"description\": \"The last port, inclusive, in the range of ports for the endpoint group that is associated with a custom routing accelerator.\"\n        }\n      ]\n    },\n    \"Protocols\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingProtocols\"\n        },\n        {\n          \"description\": \"The protocol for the endpoint group that is associated with a custom routing accelerator. The protocol can be either TCP or UDP.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FromPort\",\n    \"ToPort\",\n    \"Protocols\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-destination-configuration-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CustomRoutingDestinationConfiguration
---
