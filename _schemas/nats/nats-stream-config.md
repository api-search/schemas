---
description: Schema for configuring a NATS JetStream stream.
layout: schema
name: NATS JetStream Stream Configuration
properties_list:
- description: A unique name for the stream
  name: name
  type: string
- description: Optional description for the stream
  name: description
  type: string
- description: A list of subjects to consume, supports wildcards
  name: subjects
  type: array
- description: How messages are retained in the stream
  name: retention
  type: string
- description: Maximum number of consumers, -1 for unlimited
  name: max_consumers
  type: integer
- description: Maximum number of messages, -1 for unlimited
  name: max_msgs
  type: integer
- description: Maximum total bytes, -1 for unlimited
  name: max_bytes
  type: integer
- description: Maximum age in nanoseconds, 0 for unlimited
  name: max_age
  type: integer
- description: Maximum message size in bytes
  name: max_msg_size
  type: integer
- description: Storage backend type
  name: storage
  type: string
- description: Number of stream replicas
  name: num_replicas
  type: integer
- description: Discard policy when stream limits are reached
  name: discard
  type: string
- description: Window within which to track duplicate messages in nanoseconds
  name: duplicate_window
  type: integer
- description: Allow rollup headers to purge subjects
  name: allow_rollup_hdrs
  type: boolean
- description: Deny message deletion via API
  name: deny_delete
  type: boolean
- description: Deny stream purge via API
  name: deny_purge
  type: boolean
- description: Allow direct message access
  name: allow_direct
  type: boolean
- description: Mirror configuration for stream mirroring
  name: mirror
  type: object
- description: Sources for stream sourcing
  name: sources
  type: array
provider_name: NATS
provider_slug: nats
schema_file: json-schema/nats-stream-config.json
slug: nats-stream-config
source_filename: nats-stream-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/nats/nats-stream-config.json\",\n  \"title\": \"NATS JetStream Stream Configuration\",\n  \"description\": \"Schema for configuring a NATS JetStream stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A unique name for the stream\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description for the stream\"\n    },\n    \"subjects\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of subjects to consume, supports wildcards\"\n    },\n    \"retention\": {\n      \"type\": \"string\",\n      \"enum\": [\"limits\", \"interest\", \"workqueue\"],\n      \"default\": \"limits\",\n      \"description\": \"How messages are retained in the stream\"\n    },\n    \"max_consumers\"\
  : {\n      \"type\": \"integer\",\n      \"default\": -1,\n      \"description\": \"Maximum number of consumers, -1 for unlimited\"\n    },\n    \"max_msgs\": {\n      \"type\": \"integer\",\n      \"default\": -1,\n      \"description\": \"Maximum number of messages, -1 for unlimited\"\n    },\n    \"max_bytes\": {\n      \"type\": \"integer\",\n      \"default\": -1,\n      \"description\": \"Maximum total bytes, -1 for unlimited\"\n    },\n    \"max_age\": {\n      \"type\": \"integer\",\n      \"default\": 0,\n      \"description\": \"Maximum age in nanoseconds, 0 for unlimited\"\n    },\n    \"max_msg_size\": {\n      \"type\": \"integer\",\n      \"default\": -1,\n      \"description\": \"Maximum message size in bytes\"\n    },\n    \"storage\": {\n      \"type\": \"string\",\n      \"enum\": [\"file\", \"memory\"],\n      \"default\": \"file\",\n      \"description\": \"Storage backend type\"\n    },\n    \"num_replicas\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n\
  \      \"maximum\": 5,\n      \"default\": 1,\n      \"description\": \"Number of stream replicas\"\n    },\n    \"discard\": {\n      \"type\": \"string\",\n      \"enum\": [\"old\", \"new\"],\n      \"default\": \"old\",\n      \"description\": \"Discard policy when stream limits are reached\"\n    },\n    \"duplicate_window\": {\n      \"type\": \"integer\",\n      \"description\": \"Window within which to track duplicate messages in nanoseconds\"\n    },\n    \"allow_rollup_hdrs\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Allow rollup headers to purge subjects\"\n    },\n    \"deny_delete\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Deny message deletion via API\"\n    },\n    \"deny_purge\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Deny stream purge via API\"\n    },\n    \"allow_direct\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n  \
  \    \"description\": \"Allow direct message access\"\n    },\n    \"mirror\": {\n      \"type\": \"object\",\n      \"description\": \"Mirror configuration for stream mirroring\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"opt_start_seq\": {\n          \"type\": \"integer\"\n        },\n        \"filter_subject\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"description\": \"Sources for stream sourcing\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"opt_start_seq\": {\n            \"type\": \"integer\"\n          },\n          \"filter_subject\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nats/refs/heads/main/json-schema/nats-stream-config.json
tags:
- Cloud Native
- IoT
- Message Broker
- Microservices
- Pub Sub
title: NATS JetStream Stream Configuration
---
