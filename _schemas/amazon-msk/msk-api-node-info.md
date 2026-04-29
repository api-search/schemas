---
description: <p>The node information object.</p>
layout: schema
name: NodeInfo
properties_list:
- description: ''
  name: AddedToClusterTime
  type: object
- description: ''
  name: BrokerNodeInfo
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: NodeARN
  type: object
- description: ''
  name: NodeType
  type: object
- description: ''
  name: ZookeeperNodeInfo
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-node-info-schema.json
slug: msk-api-node-info
source_filename: msk-api-node-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-node-info-schema.json\",\n  \"title\": \"NodeInfo\",\n  \"description\": \"\\n            <p>The node information object.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AddedToClusterTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"addedToClusterTime\"\n          },\n          \"description\": \"\\n            <p>The start time.</p>\"\n        }\n      ]\n    },\n    \"BrokerNodeInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerNodeInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerNodeInfo\"\n          },\n          \"description\": \"\\n            <p>The broker node info.</p>\"\n        }\n      ]\n\
  \    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceType\"\n          },\n          \"description\": \"\\n            <p>The instance type.</p>\"\n        }\n      ]\n    },\n    \"NodeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nodeARN\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) of the node.</p>\"\n        }\n      ]\n    },\n    \"NodeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nodeType\"\n          },\n          \"description\": \"\\n            <p>The node type.</p>\"\n        }\n      ]\n    },\n    \"ZookeeperNodeInfo\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/ZookeeperNodeInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"zookeeperNodeInfo\"\n          },\n          \"description\": \"\\n            <p>The ZookeeperNodeInfo.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-node-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NodeInfo
---
