---
description: Returns the ports and associated IP addresses and ports of Amazon EC2 instances in your virtual private cloud (VPC) subnets. Custom routing is a port mapping protocol in Global Accelerator that statically associates port ranges with VPC subnets, which allows Global Accelerator to route to specific instances and ports within one or more subnets.
layout: schema
name: PortMapping
properties_list:
- description: ''
  name: AcceleratorPort
  type: object
- description: ''
  name: EndpointGroupArn
  type: object
- description: ''
  name: EndpointId
  type: object
- description: ''
  name: DestinationSocketAddress
  type: object
- description: ''
  name: Protocols
  type: object
- description: ''
  name: DestinationTrafficState
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-port-mapping-schema.json
slug: global-accelerator-port-mapping
source_filename: global-accelerator-port-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-port-mapping-schema.json\",\n  \"title\": \"PortMapping\",\n  \"description\": \"Returns the ports and associated IP addresses and ports of Amazon EC2 instances in your virtual private cloud (VPC) subnets. Custom routing is a port mapping protocol in Global Accelerator that statically associates port ranges with VPC subnets, which allows Global Accelerator to route to specific instances and ports within one or more subnets. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The accelerator port.\"\n        }\n      ]\n    },\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group.\"\n        }\n      ]\n    },\n    \"EndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The IP address of the VPC subnet (the subnet ID).\"\n        }\n      ]\n    },\n    \"DestinationSocketAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SocketAddress\"\n        },\n        {\n          \"description\": \"The EC2 instance IP address and port number in the virtual private cloud (VPC) subnet.\"\n        }\n      ]\n    },\n    \"Protocols\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingProtocols\"\n        },\n        {\n          \"description\": \"The protocols supported by the endpoint group.\"\n        }\n      ]\n    },\n    \"DestinationTrafficState\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/CustomRoutingDestinationTrafficState\"\n        },\n        {\n          \"description\": \"Indicates whether or not a port mapping destination can receive traffic. The value is either ALLOW, if traffic is allowed to the destination, or DENY, if traffic is not allowed to the destination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-port-mapping-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: PortMapping
---
