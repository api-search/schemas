---
description: Information about a BGP peer.
layout: schema
name: BGPPeer
properties_list:
- description: ''
  name: bgpPeerId
  type: object
- description: ''
  name: asn
  type: object
- description: ''
  name: authKey
  type: object
- description: ''
  name: addressFamily
  type: object
- description: ''
  name: amazonAddress
  type: object
- description: ''
  name: customerAddress
  type: object
- description: ''
  name: bgpPeerState
  type: object
- description: ''
  name: bgpStatus
  type: object
- description: ''
  name: awsDeviceV2
  type: object
- description: ''
  name: awsLogicalDeviceId
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-bgp-peer-schema.json
slug: amazon-direct-connect-bgp-peer
source_filename: amazon-direct-connect-bgp-peer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-bgp-peer-schema.json\",\n  \"title\": \"BGPPeer\",\n  \"description\": \"Information about a BGP peer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bgpPeerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BGPPeerId\"\n        },\n        {\n          \"description\": \"The ID of the BGP peer.\"\n        }\n      ]\n    },\n    \"asn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ASN\"\n        },\n        {\n          \"description\": \"The autonomous system (AS) number for Border Gateway Protocol (BGP) configuration.\"\n        }\n      ]\n    },\n    \"authKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BGPAuthKey\"\n        },\n        {\n          \"description\"\
  : \"The authentication key for BGP configuration. This string has a minimum length of 6 characters and and a maximun lenth of 80 characters.\"\n        }\n      ]\n    },\n    \"addressFamily\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressFamily\"\n        },\n        {\n          \"description\": \"The address family for the BGP peer.\"\n        }\n      ]\n    },\n    \"amazonAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonAddress\"\n        },\n        {\n          \"description\": \"The IP address assigned to the Amazon interface.\"\n        }\n      ]\n    },\n    \"customerAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerAddress\"\n        },\n        {\n          \"description\": \"The IP address assigned to the customer interface.\"\n        }\n      ]\n    },\n    \"bgpPeerState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BGPPeerState\"\
  \n        },\n        {\n          \"description\": \"<p>The state of the BGP peer. The following are the possible values:</p> <ul> <li> <p> <code>verifying</code>: The BGP peering addresses or ASN require validation before the BGP peer can be created. This state applies only to public virtual interfaces.</p> </li> <li> <p> <code>pending</code>: The BGP peer is created, and remains in this state until it is ready to be established.</p> </li> <li> <p> <code>available</code>: The BGP peer is ready to be established.</p> </li> <li> <p> <code>deleting</code>: The BGP peer is being deleted.</p> </li> <li> <p> <code>deleted</code>: The BGP peer is deleted and cannot be established.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"bgpStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BGPStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the BGP peer. The following are the possible values:</p> <ul> <li> <p> <code>up</code>: The\
  \ BGP peer is established. This state does not indicate the state of the routing function. Ensure that you are receiving routes over the BGP session.</p> </li> <li> <p> <code>down</code>: The BGP peer is down.</p> </li> <li> <p> <code>unknown</code>: The BGP peer status is not available.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"awsDeviceV2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsDeviceV2\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint that terminates the BGP peer.\"\n        }\n      ]\n    },\n    \"awsLogicalDeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsLogicalDeviceId\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint that terminates the logical connection. This device might be different than the device that terminates the physical connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-bgp-peer-schema.json
tags:
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: BGPPeer
---
