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
