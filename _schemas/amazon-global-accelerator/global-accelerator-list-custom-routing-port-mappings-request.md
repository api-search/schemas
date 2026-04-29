---
description: ListCustomRoutingPortMappingsRequest schema from Amazon Global Accelerator API
layout: schema
name: ListCustomRoutingPortMappingsRequest
properties_list:
- description: ''
  name: AcceleratorArn
  type: object
- description: ''
  name: EndpointGroupArn
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-list-custom-routing-port-mappings-request-schema.json
slug: global-accelerator-list-custom-routing-port-mappings-request
source_filename: global-accelerator-list-custom-routing-port-mappings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-list-custom-routing-port-mappings-request-schema.json\",\n  \"title\": \"ListCustomRoutingPortMappingsRequest\",\n  \"description\": \"ListCustomRoutingPortMappingsRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the accelerator to list the custom routing port mappings for.\"\n        }\n      ]\n    },\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group\
  \ to list the custom routing port mappings for.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortMappingsMaxResults\"\n        },\n        {\n          \"description\": \"The number of destination port mappings that you want to return with this call. The default value is 10.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The token for the next set of results. You receive this token from a previous call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AcceleratorArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-list-custom-routing-port-mappings-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: ListCustomRoutingPortMappingsRequest
---
