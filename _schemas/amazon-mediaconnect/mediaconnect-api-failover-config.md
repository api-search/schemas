---
description: The settings for source failover.
layout: schema
name: FailoverConfig
properties_list:
- description: ''
  name: FailoverMode
  type: object
- description: ''
  name: RecoveryWindow
  type: object
- description: ''
  name: SourcePriority
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-failover-config-schema.json
slug: mediaconnect-api-failover-config
source_filename: mediaconnect-api-failover-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-failover-config-schema.json\",\n  \"title\": \"FailoverConfig\",\n  \"description\": \"The settings for source failover.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailoverMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailoverMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"failoverMode\"\n          },\n          \"description\": \"The type of failover you choose for this flow. MERGE combines the source streams into a single stream, allowing graceful recovery from any single-source loss. FAILOVER allows switching between different streams.\"\n        }\n      ]\n    },\n    \"RecoveryWindow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"recoveryWindow\"\n          },\n          \"description\": \"Search window time to look for dash-7 packets\"\n        }\n      ]\n    },\n    \"SourcePriority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourcePriority\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourcePriority\"\n          },\n          \"description\": \"The priority you want to assign to a source. You can have a primary stream and a backup stream or two equally prioritized streams.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-failover-config-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: FailoverConfig
---
