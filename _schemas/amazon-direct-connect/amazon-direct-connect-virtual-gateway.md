---
description: Information about a virtual private gateway for a private virtual interface.
layout: schema
name: VirtualGateway
properties_list:
- description: ''
  name: virtualGatewayId
  type: object
- description: ''
  name: virtualGatewayState
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-virtual-gateway-schema.json
slug: amazon-direct-connect-virtual-gateway
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-virtual-gateway-schema.json\",\n  \"title\": \"VirtualGateway\",\n  \"description\": \"Information about a virtual private gateway for a private virtual interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualGatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayId\"\n        },\n        {\n          \"description\": \"The ID of the virtual private gateway.\"\n        }\n      ]\n    },\n    \"virtualGatewayState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayState\"\n        },\n        {\n          \"description\": \"<p>The state of the virtual private gateway. The following are the possible values:</p> <ul> <li> <p> <code>pending</code>: Initial state after creating\
  \ the virtual private gateway.</p> </li> <li> <p> <code>available</code>: Ready for use by a private virtual interface.</p> </li> <li> <p> <code>deleting</code>: Initial state after deleting the virtual private gateway.</p> </li> <li> <p> <code>deleted</code>: The virtual private gateway is deleted. The private virtual interface is unable to send traffic over this gateway.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-virtual-gateway-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: VirtualGateway
---
