---
description: Information about the virtual interface failover test.
layout: schema
name: VirtualInterfaceTestHistory
properties_list:
- description: ''
  name: testId
  type: object
- description: ''
  name: virtualInterfaceId
  type: object
- description: ''
  name: bgpPeers
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: ownerAccount
  type: object
- description: ''
  name: testDurationInMinutes
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-virtual-interface-test-history-schema.json
slug: amazon-direct-connect-virtual-interface-test-history
source_filename: amazon-direct-connect-virtual-interface-test-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-virtual-interface-test-history-schema.json\",\n  \"title\": \"VirtualInterfaceTestHistory\",\n  \"description\": \"Information about the virtual interface failover test.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"testId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TestId\"\n        },\n        {\n          \"description\": \"The ID of the virtual interface failover test.\"\n        }\n      ]\n    },\n    \"virtualInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualInterfaceId\"\n        },\n        {\n          \"description\": \"The ID of the tested virtual interface.\"\n        }\n      ]\n    },\n    \"bgpPeers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BGPPeerIdList\"\
  \n        },\n        {\n          \"description\": \"The BGP peers that were put in the DOWN state as part of the virtual interface failover test.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureTestHistoryStatus\"\n        },\n        {\n          \"description\": \"The status of the virtual interface failover test.\"\n        }\n      ]\n    },\n    \"ownerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OwnerAccount\"\n        },\n        {\n          \"description\": \"The owner ID of the tested virtual interface.\"\n        }\n      ]\n    },\n    \"testDurationInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TestDuration\"\n        },\n        {\n          \"description\": \"The time that the virtual interface failover test ran in minutes.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/StartTime\"\n        },\n        {\n          \"description\": \"The time that the virtual interface moves to the DOWN state.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndTime\"\n        },\n        {\n          \"description\": \"The time that the virtual interface moves out of the DOWN state.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-virtual-interface-test-history-schema.json
tags:
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: VirtualInterfaceTestHistory
---
