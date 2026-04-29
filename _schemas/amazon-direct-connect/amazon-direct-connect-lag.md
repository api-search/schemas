---
description: Information about a link aggregation group (LAG).
layout: schema
name: Lag
properties_list:
- description: ''
  name: connectionsBandwidth
  type: object
- description: ''
  name: numberOfConnections
  type: object
- description: ''
  name: lagId
  type: object
- description: ''
  name: ownerAccount
  type: object
- description: ''
  name: lagName
  type: object
- description: ''
  name: lagState
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: minimumLinks
  type: object
- description: ''
  name: awsDevice
  type: object
- description: ''
  name: awsDeviceV2
  type: object
- description: ''
  name: awsLogicalDeviceId
  type: object
- description: ''
  name: connections
  type: object
- description: ''
  name: allowsHostedConnections
  type: object
- description: ''
  name: jumboFrameCapable
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
  name: encryptionMode
  type: object
- description: ''
  name: macSecKeys
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-lag-schema.json
slug: amazon-direct-connect-lag
source_filename: amazon-direct-connect-lag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-lag-schema.json\",\n  \"title\": \"Lag\",\n  \"description\": \"Information about a link aggregation group (LAG).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionsBandwidth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Bandwidth\"\n        },\n        {\n          \"description\": \"The individual bandwidth of the physical connections bundled by the LAG. The possible values are 1Gbps and 10Gbps. \"\n        }\n      ]\n    },\n    \"numberOfConnections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The number of physical dedicated connections bundled by the LAG, up to a maximum of 10.\"\n        }\n      ]\n    },\n    \"lagId\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LagId\"\n        },\n        {\n          \"description\": \"The ID of the LAG.\"\n        }\n      ]\n    },\n    \"ownerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OwnerAccount\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the LAG.\"\n        }\n      ]\n    },\n    \"lagName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LagName\"\n        },\n        {\n          \"description\": \"The name of the LAG.\"\n        }\n      ]\n    },\n    \"lagState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LagState\"\n        },\n        {\n          \"description\": \"<p>The state of the LAG. The following are the possible values:</p> <ul> <li> <p> <code>requested</code>: The initial state of a LAG. The LAG stays in the requested state until the Letter\
  \ of Authorization (LOA) is available.</p> </li> <li> <p> <code>pending</code>: The LAG has been approved and is being initialized.</p> </li> <li> <p> <code>available</code>: The network link is established and the LAG is ready for use.</p> </li> <li> <p> <code>down</code>: The network link is down.</p> </li> <li> <p> <code>deleting</code>: The LAG is being deleted.</p> </li> <li> <p> <code>deleted</code>: The LAG is deleted.</p> </li> <li> <p> <code>unknown</code>: The state of the LAG is not available.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationCode\"\n        },\n        {\n          \"description\": \"The location of the LAG.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the connection is located.\"\n \
  \       }\n      ]\n    },\n    \"minimumLinks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The minimum number of physical dedicated connections that must be operational for the LAG itself to be operational.\"\n        }\n      ]\n    },\n    \"awsDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsDevice\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint that hosts the LAG.\"\n        }\n      ]\n    },\n    \"awsDeviceV2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsDeviceV2\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint that hosts the LAG.\"\n        }\n      ]\n    },\n    \"awsLogicalDeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsLogicalDeviceId\"\n        },\n        {\n          \"description\": \"The\
  \ Direct Connect endpoint that terminates the logical connection. This device might be different than the device that terminates the physical connection.\"\n        }\n      ]\n    },\n    \"connections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionList\"\n        },\n        {\n          \"description\": \"The connections bundled by the LAG.\"\n        }\n      ]\n    },\n    \"allowsHostedConnections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanFlag\"\n        },\n        {\n          \"description\": \"Indicates whether the LAG can host other connections.\"\n        }\n      ]\n    },\n    \"jumboFrameCapable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JumboFrameCapable\"\n        },\n        {\n          \"description\": \"Indicates whether jumbo frames (9001 MTU) are supported.\"\n        }\n      ]\n    },\n    \"hasLogicalRedundancy\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/HasLogicalRedundancy\"\n        },\n        {\n          \"description\": \"Indicates whether the LAG supports a secondary BGP peer in the same address family (IPv4/IPv6).\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags associated with the LAG.\"\n        }\n      ]\n    },\n    \"providerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderName\"\n        },\n        {\n          \"description\": \"The name of the service provider associated with the LAG.\"\n        }\n      ]\n    },\n    \"macSecCapable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MacSecCapable\"\n        },\n        {\n          \"description\": \"Indicates whether the LAG supports MAC Security (MACsec).\"\n        }\n      ]\n    },\n    \"encryptionMode\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionMode\"\n        },\n        {\n          \"description\": \"<p>The LAG MAC Security (MACsec) encryption mode.</p> <p>The valid values are <code>no_encrypt</code>, <code>should_encrypt</code>, and <code>must_encrypt</code>.</p>\"\n        }\n      ]\n    },\n    \"macSecKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MacSecKeyList\"\n        },\n        {\n          \"description\": \"The MAC Security (MACsec) security keys associated with the LAG.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-lag-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: Lag
---
