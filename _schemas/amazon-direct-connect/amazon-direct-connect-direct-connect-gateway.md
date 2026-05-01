---
description: Information about a Direct Connect gateway, which enables you to connect virtual interfaces and virtual private gateway or transit gateways.
layout: schema
name: DirectConnectGateway
properties_list:
- description: ''
  name: directConnectGatewayId
  type: object
- description: ''
  name: directConnectGatewayName
  type: object
- description: ''
  name: amazonSideAsn
  type: object
- description: ''
  name: ownerAccount
  type: object
- description: ''
  name: directConnectGatewayState
  type: object
- description: ''
  name: stateChangeError
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-direct-connect-gateway-schema.json
slug: amazon-direct-connect-direct-connect-gateway
source_filename: amazon-direct-connect-direct-connect-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-direct-connect-gateway-schema.json\",\n  \"title\": \"DirectConnectGateway\",\n  \"description\": \"Information about a Direct Connect gateway, which enables you to connect virtual interfaces and virtual private gateway or transit gateways.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directConnectGatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayId\"\n        },\n        {\n          \"description\": \"The ID of the Direct Connect gateway.\"\n        }\n      ]\n    },\n    \"directConnectGatewayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayName\"\n        },\n        {\n          \"description\": \"The name of the Direct Connect gateway.\"\n   \
  \     }\n      ]\n    },\n    \"amazonSideAsn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongAsn\"\n        },\n        {\n          \"description\": \"The autonomous system number (ASN) for the Amazon side of the connection.\"\n        }\n      ]\n    },\n    \"ownerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OwnerAccount\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the Direct Connect gateway.\"\n        }\n      ]\n    },\n    \"directConnectGatewayState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayState\"\n        },\n        {\n          \"description\": \"<p>The state of the Direct Connect gateway. The following are the possible values:</p> <ul> <li> <p> <code>pending</code>: The initial state after calling <a>CreateDirectConnectGateway</a>.</p> </li> <li> <p> <code>available</code>: The\
  \ Direct Connect gateway is ready for use.</p> </li> <li> <p> <code>deleting</code>: The initial state after calling <a>DeleteDirectConnectGateway</a>.</p> </li> <li> <p> <code>deleted</code>: The Direct Connect gateway is deleted and cannot pass traffic.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"stateChangeError\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateChangeError\"\n        },\n        {\n          \"description\": \"The error message if the state of an object failed to advance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-direct-connect-gateway-schema.json
tags:
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: DirectConnectGateway
---
