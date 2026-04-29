---
description: Information about a private virtual interface.
layout: schema
name: NewPrivateVirtualInterface
properties_list:
- description: ''
  name: virtualInterfaceName
  type: object
- description: ''
  name: vlan
  type: object
- description: ''
  name: asn
  type: object
- description: ''
  name: mtu
  type: object
- description: ''
  name: authKey
  type: object
- description: ''
  name: amazonAddress
  type: object
- description: ''
  name: customerAddress
  type: object
- description: ''
  name: addressFamily
  type: object
- description: ''
  name: virtualGatewayId
  type: object
- description: ''
  name: directConnectGatewayId
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: enableSiteLink
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-new-private-virtual-interface-schema.json
slug: amazon-direct-connect-new-private-virtual-interface
source_filename: amazon-direct-connect-new-private-virtual-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-new-private-virtual-interface-schema.json\",\n  \"title\": \"NewPrivateVirtualInterface\",\n  \"description\": \"Information about a private virtual interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualInterfaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualInterfaceName\"\n        },\n        {\n          \"description\": \"The name of the virtual interface assigned by the customer network. The name has a maximum of 100 characters. The following are valid characters: a-z, 0-9 and a hyphen (-).\"\n        }\n      ]\n    },\n    \"vlan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VLAN\"\n        },\n        {\n          \"description\": \"The ID of the VLAN.\"\n        }\n  \
  \    ]\n    },\n    \"asn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ASN\"\n        },\n        {\n          \"description\": \"<p>The autonomous system (AS) number for Border Gateway Protocol (BGP) configuration.</p> <p>The valid values are 1-2147483647.</p>\"\n        }\n      ]\n    },\n    \"mtu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MTU\"\n        },\n        {\n          \"description\": \"The maximum transmission unit (MTU), in bytes. The supported values are 1500 and 9001. The default value is 1500.\"\n        }\n      ]\n    },\n    \"authKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BGPAuthKey\"\n        },\n        {\n          \"description\": \"The authentication key for BGP configuration. This string has a minimum length of 6 characters and and a maximun lenth of 80 characters.\"\n        }\n      ]\n    },\n    \"amazonAddress\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/AmazonAddress\"\n        },\n        {\n          \"description\": \"The IP address assigned to the Amazon interface.\"\n        }\n      ]\n    },\n    \"customerAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerAddress\"\n        },\n        {\n          \"description\": \"The IP address assigned to the customer interface.\"\n        }\n      ]\n    },\n    \"addressFamily\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressFamily\"\n        },\n        {\n          \"description\": \"The address family for the BGP peer.\"\n        }\n      ]\n    },\n    \"virtualGatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayId\"\n        },\n        {\n          \"description\": \"The ID of the virtual private gateway.\"\n        }\n      ]\n    },\n    \"directConnectGatewayId\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayId\"\n        },\n        {\n          \"description\": \"The ID of the Direct Connect gateway.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags associated with the private virtual interface.\"\n        }\n      ]\n    },\n    \"enableSiteLink\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnableSiteLink\"\n        },\n        {\n          \"description\": \"Indicates whether to enable or disable SiteLink.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualInterfaceName\",\n    \"vlan\",\n    \"asn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-new-private-virtual-interface-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: NewPrivateVirtualInterface
---
