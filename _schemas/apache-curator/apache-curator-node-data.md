---
description: Data associated with a ZooKeeper node managed by Apache Curator, including its path, data payload, and stat metadata.
layout: schema
name: NodeData
properties_list:
- description: Full ZooKeeper path of this node.
  name: path
  type: string
- description: Node data as a Base64-encoded string or UTF-8 text.
  name: data
  type: string
- description: ZooKeeper Stat object with node metadata.
  name: stat
  type: object
provider_name: Apache Curator
provider_slug: apache-curator
schema_file: json-schema/apache-curator-node-data-schema.json
slug: apache-curator-node-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-node-data-schema.json\",\n  \"title\": \"NodeData\",\n  \"description\": \"Data associated with a ZooKeeper node managed by Apache Curator, including its path, data payload, and stat metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Full ZooKeeper path of this node.\",\n      \"example\": \"/config/app/timeout\"\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"Node data as a Base64-encoded string or UTF-8 text.\",\n      \"example\": \"30000\"\n    },\n    \"stat\": {\n      \"type\": \"object\",\n      \"description\": \"ZooKeeper Stat object with node metadata.\",\n      \"properties\": {\n        \"czxid\": {\n          \"type\": \"integer\",\n          \"description\": \"Transaction\
  \ ID that created this node.\",\n          \"example\": 1000\n        },\n        \"mzxid\": {\n          \"type\": \"integer\",\n          \"description\": \"Transaction ID of the last modification.\",\n          \"example\": 1050\n        },\n        \"ctime\": {\n          \"type\": \"integer\",\n          \"description\": \"Creation time in milliseconds since epoch.\",\n          \"example\": 1718153645993\n        },\n        \"mtime\": {\n          \"type\": \"integer\",\n          \"description\": \"Last modification time in milliseconds since epoch.\",\n          \"example\": 1718160000000\n        },\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of changes to this node data.\",\n          \"example\": 2\n        },\n        \"cversion\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of changes to the children of this node.\",\n          \"example\": 0\n        },\n        \"aversion\": {\n          \"\
  type\": \"integer\",\n          \"description\": \"Number of changes to the ACL of this node.\",\n          \"example\": 0\n        },\n        \"numChildren\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of child nodes.\",\n          \"example\": 0\n        },\n        \"dataLength\": {\n          \"type\": \"integer\",\n          \"description\": \"Length of the data field in bytes.\",\n          \"example\": 5\n        },\n        \"ephemeralOwner\": {\n          \"type\": \"integer\",\n          \"description\": \"Session ID of the owner if ephemeral, 0 otherwise.\",\n          \"example\": 0\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-node-data-schema.json
tags:
- Apache
- Distributed Coordination
- Distributed Systems
- Java
- Maven
- Open Source
- Service Discovery
- ZooKeeper
title: NodeData
---
