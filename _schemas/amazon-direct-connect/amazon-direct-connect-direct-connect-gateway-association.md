---
description: Information about an association between a Direct Connect gateway and a virtual private gateway or transit gateway.
layout: schema
name: DirectConnectGatewayAssociation
properties_list:
- description: ''
  name: directConnectGatewayId
  type: object
- description: ''
  name: directConnectGatewayOwnerAccount
  type: object
- description: ''
  name: associationState
  type: object
- description: ''
  name: stateChangeError
  type: object
- description: ''
  name: associatedGateway
  type: object
- description: ''
  name: associationId
  type: object
- description: ''
  name: allowedPrefixesToDirectConnectGateway
  type: object
- description: ''
  name: virtualGatewayId
  type: object
- description: ''
  name: virtualGatewayRegion
  type: object
- description: ''
  name: virtualGatewayOwnerAccount
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-direct-connect-gateway-association-schema.json
slug: amazon-direct-connect-direct-connect-gateway-association
source_filename: amazon-direct-connect-direct-connect-gateway-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-direct-connect-gateway-association-schema.json\",\n  \"title\": \"DirectConnectGatewayAssociation\",\n  \"description\": \"Information about an association between a Direct Connect gateway and a virtual private gateway or transit gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directConnectGatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayId\"\n        },\n        {\n          \"description\": \"The ID of the Direct Connect gateway.\"\n        }\n      ]\n    },\n    \"directConnectGatewayOwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OwnerAccount\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the\
  \ associated gateway.\"\n        }\n      ]\n    },\n    \"associationState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayAssociationState\"\n        },\n        {\n          \"description\": \"<p>The state of the association. The following are the possible values:</p> <ul> <li> <p> <code>associating</code>: The initial state after calling <a>CreateDirectConnectGatewayAssociation</a>.</p> </li> <li> <p> <code>associated</code>: The Direct Connect gateway and virtual private gateway or transit gateway are successfully associated and ready to pass traffic.</p> </li> <li> <p> <code>disassociating</code>: The initial state after calling <a>DeleteDirectConnectGatewayAssociation</a>.</p> </li> <li> <p> <code>disassociated</code>: The virtual private gateway or transit gateway is disassociated from the Direct Connect gateway. Traffic flow between the Direct Connect gateway and virtual private gateway or transit gateway is stopped.</p> </li>\
  \ <li> <p> <code>updating</code>: The CIDR blocks for the virtual private gateway or transit gateway are currently being updated. This could be new CIDR blocks added or current CIDR blocks removed.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"stateChangeError\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateChangeError\"\n        },\n        {\n          \"description\": \"The error message if the state of an object failed to advance.\"\n        }\n      ]\n    },\n    \"associatedGateway\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociatedGateway\"\n        },\n        {\n          \"description\": \"Information about the associated gateway.\"\n        }\n      ]\n    },\n    \"associationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayAssociationId\"\n        },\n        {\n          \"description\": \"The ID of the Direct Connect gateway association.\"\
  \n        }\n      ]\n    },\n    \"allowedPrefixesToDirectConnectGateway\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RouteFilterPrefixList\"\n        },\n        {\n          \"description\": \"The Amazon VPC prefixes to advertise to the Direct Connect gateway.\"\n        }\n      ]\n    },\n    \"virtualGatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayId\"\n        },\n        {\n          \"description\": \"The ID of the virtual private gateway. Applies only to private virtual interfaces.\"\n        }\n      ]\n    },\n    \"virtualGatewayRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayRegion\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the virtual private gateway is located.\"\n        }\n      ]\n    },\n    \"virtualGatewayOwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/OwnerAccount\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the virtual private gateway.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-direct-connect-gateway-association-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: DirectConnectGatewayAssociation
---
