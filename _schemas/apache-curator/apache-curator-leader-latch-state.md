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
source_filename: apache-curator-leader-latch-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-leader-latch-state-schema.json\",\n  \"title\": \"LeaderLatchState\",\n  \"description\": \"State of a LeaderLatch participant in Apache Curator leader election.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Participant ID used in the leader election.\",\n      \"example\": \"node-01\"\n    },\n    \"isLeader\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this participant is currently the leader.\",\n      \"example\": true\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"LeaderLatch lifecycle state.\",\n      \"enum\": [\n        \"LATENT\",\n        \"STARTED\",\n        \"CLOSED\"\n      ],\n      \"example\": \"STARTED\"\n    },\n    \"path\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"ZooKeeper path used for leader election.\",\n      \"example\": \"/services/leader\"\n    },\n    \"participants\": {\n      \"type\": \"array\",\n      \"description\": \"All participants in the election.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"node-01\"\n          },\n          \"isLeader\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-leader-latch-state-schema.json
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
