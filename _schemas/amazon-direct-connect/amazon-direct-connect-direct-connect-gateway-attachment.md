---
description: Information about an attachment between a Direct Connect gateway and a virtual interface.
layout: schema
name: DirectConnectGatewayAttachment
properties_list:
- description: ''
  name: directConnectGatewayId
  type: object
- description: ''
  name: virtualInterfaceId
  type: object
- description: ''
  name: virtualInterfaceRegion
  type: object
- description: ''
  name: virtualInterfaceOwnerAccount
  type: object
- description: ''
  name: attachmentState
  type: object
- description: ''
  name: attachmentType
  type: object
- description: ''
  name: stateChangeError
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-direct-connect-gateway-attachment-schema.json
slug: amazon-direct-connect-direct-connect-gateway-attachment
source_filename: amazon-direct-connect-direct-connect-gateway-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-direct-connect-gateway-attachment-schema.json\",\n  \"title\": \"DirectConnectGatewayAttachment\",\n  \"description\": \"Information about an attachment between a Direct Connect gateway and a virtual interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directConnectGatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayId\"\n        },\n        {\n          \"description\": \"The ID of the Direct Connect gateway.\"\n        }\n      ]\n    },\n    \"virtualInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualInterfaceId\"\n        },\n        {\n          \"description\": \"The ID of the virtual interface.\"\n        }\n      ]\n    },\n    \"virtualInterfaceRegion\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualInterfaceRegion\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the virtual interface is located.\"\n        }\n      ]\n    },\n    \"virtualInterfaceOwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OwnerAccount\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the virtual interface.\"\n        }\n      ]\n    },\n    \"attachmentState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayAttachmentState\"\n        },\n        {\n          \"description\": \"<p>The state of the attachment. The following are the possible values:</p> <ul> <li> <p> <code>attaching</code>: The initial state after a virtual interface is created using the Direct Connect gateway.</p> </li> <li> <p> <code>attached</code>: The Direct Connect\
  \ gateway and virtual interface are attached and ready to pass traffic.</p> </li> <li> <p> <code>detaching</code>: The initial state after calling <a>DeleteVirtualInterface</a>.</p> </li> <li> <p> <code>detached</code>: The virtual interface is detached from the Direct Connect gateway. Traffic flow between the Direct Connect gateway and virtual interface is stopped.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"attachmentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayAttachmentType\"\n        },\n        {\n          \"description\": \"The type of attachment.\"\n        }\n      ]\n    },\n    \"stateChangeError\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateChangeError\"\n        },\n        {\n          \"description\": \"The error message if the state of an object failed to advance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-direct-connect-gateway-attachment-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: DirectConnectGatewayAttachment
---
