---
description: The port mappings for a specified endpoint IP address (destination).
layout: schema
name: DestinationPortMapping
properties_list:
- description: ''
  name: AcceleratorArn
  type: object
- description: ''
  name: AcceleratorSocketAddresses
  type: object
- description: ''
  name: EndpointGroupArn
  type: object
- description: ''
  name: EndpointId
  type: object
- description: ''
  name: EndpointGroupRegion
  type: object
- description: ''
  name: DestinationSocketAddress
  type: object
- description: ''
  name: IpAddressType
  type: object
- description: ''
  name: DestinationTrafficState
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-destination-port-mapping-schema.json
slug: global-accelerator-destination-port-mapping
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-destination-port-mapping-schema.json\",\n  \"title\": \"DestinationPortMapping\",\n  \"description\": \"The port mappings for a specified endpoint IP address (destination).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the custom routing accelerator that you have port mappings for.\"\n        }\n      ]\n    },\n    \"AcceleratorSocketAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SocketAddresses\"\n        },\n        {\n          \"description\": \"The IP address/port combinations (sockets) that map to a given destination socket\
  \ address.\"\n        }\n      ]\n    },\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group.\"\n        }\n      ]\n    },\n    \"EndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The ID for the virtual private cloud (VPC) subnet.\"\n        }\n      ]\n    },\n    \"EndpointGroupRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region for the endpoint group.\"\n        }\n      ]\n    },\n    \"DestinationSocketAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SocketAddress\"\n        },\n        {\n          \"description\": \"The endpoint\
  \ IP address/port combination for traffic received on the accelerator socket address.\"\n        }\n      ]\n    },\n    \"IpAddressType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressType\"\n        },\n        {\n          \"description\": \"The IP address type that an accelerator supports. For a custom routing accelerator, the value must be IPV4.\"\n        }\n      ]\n    },\n    \"DestinationTrafficState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingDestinationTrafficState\"\n        },\n        {\n          \"description\": \"Indicates whether or not a port mapping destination can receive traffic. The value is either ALLOW, if traffic is allowed to the destination, or DENY, if traffic is not allowed to the destination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-destination-port-mapping-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: DestinationPortMapping
---
