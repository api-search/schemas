---
description: Configuration and state for an Apache Curator InterProcessMutex distributed lock.
layout: schema
name: DistributedLock
properties_list:
- description: ZooKeeper path used as the lock node.
  name: path
  type: string
- description: Whether the lock is currently acquired by this process.
  name: acquired
  type: boolean
- description: Number of times the current thread holds the lock (reentrant count).
  name: threadCount
  type: integer
- description: Actual ZooKeeper ephemeral node path created for this lock acquisition.
  name: lockPath
  type: string
provider_name: Apache Curator
provider_slug: apache-curator
schema_file: json-schema/apache-curator-distributed-lock-schema.json
slug: apache-curator-distributed-lock
source_filename: apache-curator-distributed-lock-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-distributed-lock-schema.json\",\n  \"title\": \"DistributedLock\",\n  \"description\": \"Configuration and state for an Apache Curator InterProcessMutex distributed lock.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"ZooKeeper path used as the lock node.\",\n      \"example\": \"/locks/resource-a\"\n    },\n    \"acquired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the lock is currently acquired by this process.\",\n      \"example\": true\n    },\n    \"threadCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times the current thread holds the lock (reentrant count).\",\n      \"minimum\": 0,\n      \"example\": 1\n    },\n    \"lockPath\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Actual ZooKeeper ephemeral node path created for this lock acquisition.\",\n      \"example\": \"/locks/resource-a/_c_abc123-lock-0000000001\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-distributed-lock-schema.json
tags:
- Apache
- Distributed Coordination
- Distributed Systems
- Java
- Maven
- Open Source
- Service Discovery
- ZooKeeper
title: DistributedLock
---
