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
