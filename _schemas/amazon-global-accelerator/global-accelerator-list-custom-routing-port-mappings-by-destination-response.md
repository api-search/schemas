---
description: ListCustomRoutingPortMappingsByDestinationResponse schema from Amazon Global Accelerator API
layout: schema
name: ListCustomRoutingPortMappingsByDestinationResponse
properties_list:
- description: ''
  name: DestinationPortMappings
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-list-custom-routing-port-mappings-by-destination-response-schema.json
slug: global-accelerator-list-custom-routing-port-mappings-by-destination-response
source_filename: global-accelerator-list-custom-routing-port-mappings-by-destination-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-list-custom-routing-port-mappings-by-destination-response-schema.json\",\n  \"title\": \"ListCustomRoutingPortMappingsByDestinationResponse\",\n  \"description\": \"ListCustomRoutingPortMappingsByDestinationResponse schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationPortMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationPortMappings\"\n        },\n        {\n          \"description\": \"The port mappings for the endpoint IP address that you specified in the request.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The token\
  \ for the next set of results. You receive this token from a previous call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-list-custom-routing-port-mappings-by-destination-response-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: ListCustomRoutingPortMappingsByDestinationResponse
---
