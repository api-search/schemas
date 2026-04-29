---
description: Information about an interconnect.
layout: schema
name: Interconnect
properties_list:
- description: ''
  name: interconnectId
  type: object
- description: ''
  name: interconnectName
  type: object
- description: ''
  name: interconnectState
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
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-interconnect-schema.json
slug: amazon-direct-connect-interconnect
source_filename: amazon-direct-connect-interconnect-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-interconnect-schema.json\",\n  \"title\": \"Interconnect\",\n  \"description\": \"Information about an interconnect.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"interconnectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterconnectId\"\n        },\n        {\n          \"description\": \"The ID of the interconnect.\"\n        }\n      ]\n    },\n    \"interconnectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterconnectName\"\n        },\n        {\n          \"description\": \"The name of the interconnect.\"\n        }\n      ]\n    },\n    \"interconnectState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterconnectState\"\n        },\n        {\n   \
  \       \"description\": \"<p>The state of the interconnect. The following are the possible values:</p> <ul> <li> <p> <code>requested</code>: The initial state of an interconnect. The interconnect stays in the requested state until the Letter of Authorization (LOA) is sent to the customer.</p> </li> <li> <p> <code>pending</code>: The interconnect is approved, and is being initialized.</p> </li> <li> <p> <code>available</code>: The network link is up, and the interconnect is ready for use.</p> </li> <li> <p> <code>down</code>: The network link is down.</p> </li> <li> <p> <code>deleting</code>: The interconnect is being deleted.</p> </li> <li> <p> <code>deleted</code>: The interconnect is deleted.</p> </li> <li> <p> <code>unknown</code>: The state of the interconnect is not available.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\n        },\n        {\n          \"description\": \"The\
  \ Amazon Web Services Region where the connection is located.\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationCode\"\n        },\n        {\n          \"description\": \"The location of the connection.\"\n        }\n      ]\n    },\n    \"bandwidth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Bandwidth\"\n        },\n        {\n          \"description\": \"The bandwidth of the connection.\"\n        }\n      ]\n    },\n    \"loaIssueTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoaIssueTime\"\n        },\n        {\n          \"description\": \"The time of the most recent call to <a>DescribeLoa</a> for this connection.\"\n        }\n      ]\n    },\n    \"lagId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LagId\"\n        },\n        {\n          \"description\": \"The ID of the LAG.\"\n      \
  \  }\n      ]\n    },\n    \"awsDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsDevice\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint on which the physical connection terminates.\"\n        }\n      ]\n    },\n    \"jumboFrameCapable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JumboFrameCapable\"\n        },\n        {\n          \"description\": \"Indicates whether jumbo frames (9001 MTU) are supported.\"\n        }\n      ]\n    },\n    \"awsDeviceV2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsDeviceV2\"\n        },\n        {\n          \"description\": \"The Direct Connect endpoint that terminates the physical connection.\"\n        }\n      ]\n    },\n    \"awsLogicalDeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsLogicalDeviceId\"\n        },\n        {\n          \"description\": \"The\
  \ Direct Connect endpoint that terminates the logical connection. This device might be different than the device that terminates the physical connection.\"\n        }\n      ]\n    },\n    \"hasLogicalRedundancy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HasLogicalRedundancy\"\n        },\n        {\n          \"description\": \"Indicates whether the interconnect supports a secondary BGP in the same address family (IPv4/IPv6).\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags associated with the interconnect.\"\n        }\n      ]\n    },\n    \"providerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderName\"\n        },\n        {\n          \"description\": \"The name of the service provider associated with the interconnect.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-interconnect-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: Interconnect
---
