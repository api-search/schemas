---
description: DenyCustomRoutingTrafficRequest schema from Amazon Global Accelerator API
layout: schema
name: DenyCustomRoutingTrafficRequest
properties_list:
- description: ''
  name: EndpointGroupArn
  type: object
- description: ''
  name: EndpointId
  type: object
- description: ''
  name: DestinationAddresses
  type: object
- description: ''
  name: DestinationPorts
  type: object
- description: ''
  name: DenyAllTrafficToEndpoint
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-deny-custom-routing-traffic-request-schema.json
slug: global-accelerator-deny-custom-routing-traffic-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-deny-custom-routing-traffic-request-schema.json\",\n  \"title\": \"DenyCustomRoutingTrafficRequest\",\n  \"description\": \"DenyCustomRoutingTrafficRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group.\"\n        }\n      ]\n    },\n    \"EndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"An ID for the endpoint. For custom routing accelerators, this is the virtual private cloud (VPC) subnet ID.\"\n \
  \       }\n      ]\n    },\n    \"DestinationAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationAddresses\"\n        },\n        {\n          \"description\": \"A list of specific Amazon EC2 instance IP addresses (destination addresses) in a subnet that you want to prevent from receiving traffic. The IP addresses must be a subset of the IP addresses allowed for the VPC subnet associated with the endpoint group.\"\n        }\n      ]\n    },\n    \"DestinationPorts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationPorts\"\n        },\n        {\n          \"description\": \"A list of specific Amazon EC2 instance ports (destination ports) in a subnet endpoint that you want to prevent from receiving traffic.\"\n        }\n      ]\n    },\n    \"DenyAllTrafficToEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericBoolean\"\n        },\n        {\n          \"\
  description\": \"<p>Indicates whether all destination IP addresses and ports for a specified VPC subnet endpoint <i>cannot</i> receive traffic from a custom routing accelerator. The value is TRUE or FALSE. </p> <p>When set to TRUE, <i>no</i> destinations in the custom routing VPC subnet can receive traffic. Note that you cannot specify destination IP addresses and ports when the value is set to TRUE.</p> <p>When set to FALSE (or not specified), you <i>must</i> specify a list of destination IP addresses that cannot receive traffic. A list of ports is optional. If you don't specify a list of ports, the ports that can accept traffic is the same as the ports configured for the endpoint group.</p> <p>The default value is FALSE.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointGroupArn\",\n    \"EndpointId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-deny-custom-routing-traffic-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: DenyCustomRoutingTrafficRequest
---
