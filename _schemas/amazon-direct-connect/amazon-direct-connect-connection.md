---
description: Information about an Direct Connect connection.
layout: schema
name: Connection
properties_list:
- description: ''
  name: ownerAccount
  type: object
- description: ''
  name: connectionId
  type: object
- description: ''
  name: connectionName
  type: object
- description: ''
  name: connectionState
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: bandwidth
  type: object
- description: ''
  name: vlan
  type: object
- description: ''
  name: partnerName
  type: object
- description: ''
  name: loaIssueTime
  type: object
- description: ''
  name: lagId
  type: object
- description: ''
  name: awsDevice
  type: object
- description: ''
  name: jumboFrameCapable
  type: object
- description: ''
  name: awsDeviceV2
  type: object
- description: ''
  name: awsLogicalDeviceId
  type: object
- description: ''
  name: hasLogicalRedundancy
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: providerName
  type: object
- description: ''
  name: macSecCapable
  type: object
- description: ''
  name: portEncryptionStatus
  type: object
- description: ''
  name: encryptionMode
  type: object
- description: ''
  name: macSecKeys
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-connection-schema.json
slug: amazon-direct-connect-connection
source_filename: amazon-direct-connect-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-connection-schema.json\",\n  \"title\": \"Connection\",\n  \"description\": \"Information about an Direct Connect connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ownerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OwnerAccount\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the connection.\"\n        }\n      ]\n    },\n    \"connectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionId\"\n        },\n        {\n          \"description\": \"The ID of the connection.\"\n        }\n      ]\n    },\n    \"connectionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionName\"\n\
  \        },\n        {\n          \"description\": \"The name of the connection.\"\n        }\n      ]\n    },\n    \"connectionState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionState\"\n        },\n        {\n          \"description\": \"<p>The state of the connection. The following are the possible values:</p> <ul> <li> <p> <code>ordering</code>: The initial state of a hosted connection provisioned on an interconnect. The connection stays in the ordering state until the owner of the hosted connection confirms or declines the connection order.</p> </li> <li> <p> <code>requested</code>: The initial state of a standard connection. The connection stays in the requested state until the Letter of Authorization (LOA) is sent to the customer.</p> </li> <li> <p> <code>pending</code>: The connection has been approved and is being initialized.</p> </li> <li> <p> <code>available</code>: The network link is up and the connection is ready for use.</p>\
  \ </li> <li> <p> <code>down</code>: The network link is down.</p> </li> <li> <p> <code>deleting</code>: The connection is being deleted.</p> </li> <li> <p> <code>deleted</code>: The connection has been deleted.</p> </li> <li> <p> <code>rejected</code>: A hosted connection in the <code>ordering</code> state enters the <code>rejected</code> state if it is deleted by the customer.</p> </li> <li> <p> <code>unknown</code>: The state of the connection is not available.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the connection is located.\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationCode\"\n        },\n        {\n          \"description\": \"The location of the connection.\"\n        }\n      ]\n    },\n    \"bandwidth\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Bandwidth\"\n        },\n        {\n          \"description\": \"The bandwidth of the connection.\"\n        }\n      ]\n    },\n    \"vlan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VLAN\"\n        },\n        {\n          \"description\": \"The ID of the VLAN.\"\n        }\n      ]\n    },\n    \"partnerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartnerName\"\n        },\n        {\n          \"description\": \"The name of the Direct Connect service provider associated with the connection.\"\n        }\n      ]\n    },\n    \"loaIssueTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoaIssueTime\"\n        },\n        {\n          \"description\": \"The time of the most recent call to <a>DescribeLoa</a> for this connection.\"\n        }\n      ]\n    },\n    \"lagId\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/LagId\"\n        },\n        {\n          \"description\": \"The ID of the LAG.\"\n        }\n      ]\n    },\n    \"awsDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsDevice\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint on which the physical connection terminates.\"\n        }\n      ]\n    },\n    \"jumboFrameCapable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JumboFrameCapable\"\n        },\n        {\n          \"description\": \"Indicates whether jumbo frames (9001 MTU) are supported.\"\n        }\n      ]\n    },\n    \"awsDeviceV2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsDeviceV2\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint that terminates the physical connection.\"\n        }\n      ]\n    },\n    \"awsLogicalDeviceId\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsLogicalDeviceId\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint that terminates the logical connection. This device might be different than the device that terminates the physical connection.\"\n        }\n      ]\n    },\n    \"hasLogicalRedundancy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HasLogicalRedundancy\"\n        },\n        {\n          \"description\": \"Indicates whether the connection supports a secondary BGP peer in the same address family (IPv4/IPv6).\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags associated with the connection.\"\n        }\n      ]\n    },\n    \"providerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderName\"\n        },\n  \
  \      {\n          \"description\": \"The name of the service provider associated with the connection.\"\n        }\n      ]\n    },\n    \"macSecCapable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MacSecCapable\"\n        },\n        {\n          \"description\": \"Indicates whether the connection supports MAC Security (MACsec).\"\n        }\n      ]\n    },\n    \"portEncryptionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortEncryptionStatus\"\n        },\n        {\n          \"description\": \"<p>The MAC Security (MACsec) port link status of the connection.</p> <p>The valid values are <code>Encryption Up</code>, which means that there is an active Connection Key Name, or <code>Encryption Down</code>.</p>\"\n        }\n      ]\n    },\n    \"encryptionMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionMode\"\n        },\n        {\n          \"description\": \"\
  <p>The MAC Security (MACsec) connection encryption mode.</p> <p>The valid values are <code>no_encrypt</code>, <code>should_encrypt</code>, and <code>must_encrypt</code>.</p>\"\n        }\n      ]\n    },\n    \"macSecKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MacSecKeyList\"\n        },\n        {\n          \"description\": \"The MAC Security (MACsec) security keys associated with the connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-connection-schema.json
tags:
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: Connection
---
