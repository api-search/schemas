---
description: Lifecycle state of a source server
layout: schema
name: LifeCycle
properties_list:
- description: Current lifecycle state
  name: state
  type: string
- description: Date/time the server was added to the service
  name: addedToServiceDateTime
  type: string
- description: Date/time the first replication byte was received
  name: firstByteDateTime
  type: string
- description: Elapsed duration of replication
  name: elapsedReplicationDuration
  type: string
- description: Date/time the agent last communicated with the service
  name: lastSeenByServiceDateTime
  type: string
- description: lastTestInitiated
  name: lastTestInitiated
  type: string
- description: lastTestReverted
  name: lastTestReverted
  type: string
- description: lastTestFinalized
  name: lastTestFinalized
  type: string
- description: lastCutoverInitiated
  name: lastCutoverInitiated
  type: string
- description: lastCutoverReverted
  name: lastCutoverReverted
  type: string
- description: lastCutoverFinalized
  name: lastCutoverFinalized
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-life-cycle-schema.json
slug: application-migration-service-life-cycle
source_filename: application-migration-service-life-cycle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-life-cycle-schema.json\",\n  \"title\": \"LifeCycle\",\n  \"description\": \"Lifecycle state of a source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle state\"\n    },\n    \"addedToServiceDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time the server was added to the service\"\n    },\n    \"firstByteDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time the first replication byte was received\"\n    },\n    \"elapsedReplicationDuration\": {\n      \"type\": \"string\",\n      \"description\": \"Elapsed duration of replication\"\n    },\n    \"lastSeenByServiceDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time\
  \ the agent last communicated with the service\"\n    },\n    \"lastTestInitiated\": {\n      \"type\": \"string\",\n      \"description\": \"lastTestInitiated\"\n    },\n    \"lastTestReverted\": {\n      \"type\": \"string\",\n      \"description\": \"lastTestReverted\"\n    },\n    \"lastTestFinalized\": {\n      \"type\": \"string\",\n      \"description\": \"lastTestFinalized\"\n    },\n    \"lastCutoverInitiated\": {\n      \"type\": \"string\",\n      \"description\": \"lastCutoverInitiated\"\n    },\n    \"lastCutoverReverted\": {\n      \"type\": \"string\",\n      \"description\": \"lastCutoverReverted\"\n    },\n    \"lastCutoverFinalized\": {\n      \"type\": \"string\",\n      \"description\": \"lastCutoverFinalized\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-life-cycle-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: LifeCycle
---
