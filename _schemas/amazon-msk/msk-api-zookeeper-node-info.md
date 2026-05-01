---
description: <p>Zookeeper node information.</p>
layout: schema
name: ZookeeperNodeInfo
properties_list:
- description: ''
  name: AttachedENIId
  type: object
- description: ''
  name: ClientVpcIpAddress
  type: object
- description: ''
  name: Endpoints
  type: object
- description: ''
  name: ZookeeperId
  type: object
- description: ''
  name: ZookeeperVersion
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-zookeeper-node-info-schema.json
slug: msk-api-zookeeper-node-info
source_filename: msk-api-zookeeper-node-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-zookeeper-node-info-schema.json\",\n  \"title\": \"ZookeeperNodeInfo\",\n  \"description\": \"\\n            <p>Zookeeper node information.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttachedENIId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attachedENIId\"\n          },\n          \"description\": \"\\n            <p>The attached elastic network interface of the broker.</p>\"\n        }\n      ]\n    },\n    \"ClientVpcIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientVpcIpAddress\"\n          },\n          \"description\": \"\\n            <p>The\
  \ virtual private cloud (VPC) IP address of the client.</p>\"\n        }\n      ]\n    },\n    \"Endpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"endpoints\"\n          },\n          \"description\": \"\\n            <p>Endpoints for accessing the ZooKeeper.</p>\"\n        }\n      ]\n    },\n    \"ZookeeperId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"zookeeperId\"\n          },\n          \"description\": \"\\n            <p>The role-specific ID for Zookeeper.</p>\"\n        }\n      ]\n    },\n    \"ZookeeperVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"zookeeperVersion\"\n          },\n          \"description\": \"\\\
  n            <p>The version of Zookeeper.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-zookeeper-node-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ZookeeperNodeInfo
---
