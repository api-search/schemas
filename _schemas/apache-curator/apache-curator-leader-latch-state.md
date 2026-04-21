---
description: State of a LeaderLatch participant in Apache Curator leader election.
layout: schema
name: LeaderLatchState
properties_list:
- description: Participant ID used in the leader election.
  name: id
  type: string
- description: Whether this participant is currently the leader.
  name: isLeader
  type: boolean
- description: LeaderLatch lifecycle state.
  name: state
  type: string
- description: ZooKeeper path used for leader election.
  name: path
  type: string
- description: All participants in the election.
  name: participants
  type: array
provider_name: Apache Curator
provider_slug: apache-curator
schema_file: json-schema/apache-curator-leader-latch-state-schema.json
slug: apache-curator-leader-latch-state
tags:
- Apache
- Distributed Coordination
- Distributed Systems
- Java
- Maven
- Open Source
- Service Discovery
- ZooKeeper
title: LeaderLatchState
---
