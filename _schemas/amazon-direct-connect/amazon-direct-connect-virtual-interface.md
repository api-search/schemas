---
description: Information about a virtual interface.
layout: schema
name: VirtualInterface
properties_list:
- description: ''
  name: ownerAccount
  type: object
- description: ''
  name: virtualInterfaceId
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: connectionId
  type: object
- description: ''
  name: virtualInterfaceType
  type: object
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
  name: amazonSideAsn
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
  name: virtualInterfaceState
  type: object
- description: ''
  name: customerRouterConfig
  type: object
- description: ''
  name: mtu
  type: object
- description: ''
  name: jumboFrameCapable
  type: object
- description: ''
  name: virtualGatewayId
  type: object
- description: ''
  name: directConnectGatewayId
  type: object
- description: ''
  name: routeFilterPrefixes
  type: object
- description: ''
  name: bgpPeers
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: awsDeviceV2
  type: object
- description: ''
  name: awsLogicalDeviceId
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: siteLinkEnabled
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-virtual-interface-schema.json
slug: amazon-direct-connect-virtual-interface
source_filename: amazon-direct-connect-virtual-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-virtual-interface-schema.json\",\n  \"title\": \"VirtualInterface\",\n  \"description\": \"Information about a virtual interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ownerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OwnerAccount\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the virtual interface.\"\n        }\n      ]\n    },\n    \"virtualInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualInterfaceId\"\n        },\n        {\n          \"description\": \"The ID of the virtual interface.\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationCode\"\
  \n        },\n        {\n          \"description\": \"The location of the connection.\"\n        }\n      ]\n    },\n    \"connectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionId\"\n        },\n        {\n          \"description\": \"The ID of the connection.\"\n        }\n      ]\n    },\n    \"virtualInterfaceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualInterfaceType\"\n        },\n        {\n          \"description\": \"The type of virtual interface. The possible values are <code>private</code> and <code>public</code>.\"\n        }\n      ]\n    },\n    \"virtualInterfaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualInterfaceName\"\n        },\n        {\n          \"description\": \"The name of the virtual interface assigned by the customer network. The name has a maximum of 100 characters. The following are valid characters: a-z, 0-9 and a\
  \ hyphen (-).\"\n        }\n      ]\n    },\n    \"vlan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VLAN\"\n        },\n        {\n          \"description\": \"The ID of the VLAN.\"\n        }\n      ]\n    },\n    \"asn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ASN\"\n        },\n        {\n          \"description\": \"<p>The autonomous system (AS) number for Border Gateway Protocol (BGP) configuration.</p> <p>The valid values are 1-2147483647.</p>\"\n        }\n      ]\n    },\n    \"amazonSideAsn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongAsn\"\n        },\n        {\n          \"description\": \"The autonomous system number (ASN) for the Amazon side of the connection.\"\n        }\n      ]\n    },\n    \"authKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BGPAuthKey\"\n        },\n        {\n          \"description\": \"The authentication\
  \ key for BGP configuration. This string has a minimum length of 6 characters and and a maximun lenth of 80 characters.\"\n        }\n      ]\n    },\n    \"amazonAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonAddress\"\n        },\n        {\n          \"description\": \"The IP address assigned to the Amazon interface.\"\n        }\n      ]\n    },\n    \"customerAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerAddress\"\n        },\n        {\n          \"description\": \"The IP address assigned to the customer interface.\"\n        }\n      ]\n    },\n    \"addressFamily\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressFamily\"\n        },\n        {\n          \"description\": \"The address family for the BGP peer.\"\n        }\n      ]\n    },\n    \"virtualInterfaceState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualInterfaceState\"\
  \n        },\n        {\n          \"description\": \"<p>The state of the virtual interface. The following are the possible values:</p> <ul> <li> <p> <code>confirming</code>: The creation of the virtual interface is pending confirmation from the virtual interface owner. If the owner of the virtual interface is different from the owner of the connection on which it is provisioned, then the virtual interface will remain in this state until it is confirmed by the virtual interface owner.</p> </li> <li> <p> <code>verifying</code>: This state only applies to public virtual interfaces. Each public virtual interface needs validation before the virtual interface can be created.</p> </li> <li> <p> <code>pending</code>: A virtual interface is in this state from the time that it is created until the virtual interface is ready to forward traffic.</p> </li> <li> <p> <code>available</code>: A virtual interface that is able to forward traffic.</p> </li> <li> <p> <code>down</code>: A virtual interface\
  \ that is BGP down.</p> </li> <li> <p> <code>deleting</code>: A virtual interface is in this state immediately after calling <a>DeleteVirtualInterface</a> until it can no longer forward traffic.</p> </li> <li> <p> <code>deleted</code>: A virtual interface that cannot forward traffic.</p> </li> <li> <p> <code>rejected</code>: The virtual interface owner has declined creation of the virtual interface. If a virtual interface in the <code>Confirming</code> state is deleted by the virtual interface owner, the virtual interface enters the <code>Rejected</code> state.</p> </li> <li> <p> <code>unknown</code>: The state of the virtual interface is not available.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"customerRouterConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RouterConfig\"\n        },\n        {\n          \"description\": \"The customer router configuration.\"\n        }\n      ]\n    },\n    \"mtu\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/MTU\"\n        },\n        {\n          \"description\": \"The maximum transmission unit (MTU), in bytes. The supported values are 1500 and 9001. The default value is 1500.\"\n        }\n      ]\n    },\n    \"jumboFrameCapable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JumboFrameCapable\"\n        },\n        {\n          \"description\": \"Indicates whether jumbo frames (9001 MTU) are supported.\"\n        }\n      ]\n    },\n    \"virtualGatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayId\"\n        },\n        {\n          \"description\": \"The ID of the virtual private gateway. Applies only to private virtual interfaces.\"\n        }\n      ]\n    },\n    \"directConnectGatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectConnectGatewayId\"\n        },\n        {\n          \"description\": \"The ID of the\
  \ Direct Connect gateway.\"\n        }\n      ]\n    },\n    \"routeFilterPrefixes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RouteFilterPrefixList\"\n        },\n        {\n          \"description\": \"The routes to be advertised to the Amazon Web Services network in this Region. Applies to public virtual interfaces.\"\n        }\n      ]\n    },\n    \"bgpPeers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BGPPeerList\"\n        },\n        {\n          \"description\": \"The BGP peers configured on this virtual interface.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the virtual interface is located.\"\n        }\n      ]\n    },\n    \"awsDeviceV2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsDeviceV2\"\
  \n        },\n        {\n          \"description\": \"The Direct Connect endpoint that terminates the physical connection.\"\n        }\n      ]\n    },\n    \"awsLogicalDeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsLogicalDeviceId\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint that terminates the logical connection. This device might be different than the device that terminates the physical connection.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags associated with the virtual interface.\"\n        }\n      ]\n    },\n    \"siteLinkEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SiteLinkEnabled\"\n        },\n        {\n          \"description\": \"Indicates whether SiteLink is enabled.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-virtual-interface-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: VirtualInterface
---
