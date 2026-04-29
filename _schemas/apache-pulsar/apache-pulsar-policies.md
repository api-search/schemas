---
description: Policies schema from Apache Pulsar
layout: schema
name: Policies
properties_list:
- description: ''
  name: replication_clusters
  type: array
- description: ''
  name: bundles
  type: object
- description: ''
  name: retention_policies
  type: object
- description: ''
  name: schema_auto_update_compatibility_strategy
  type: string
- description: ''
  name: message_ttl_in_seconds
  type: integer
- description: ''
  name: max_producers_per_topic
  type: integer
- description: ''
  name: max_consumers_per_topic
  type: integer
- description: ''
  name: max_consumers_per_subscription
  type: integer
- description: ''
  name: backlog_quota_map
  type: object
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/apache-pulsar-policies-schema.json
slug: apache-pulsar-policies
source_filename: apache-pulsar-policies-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-policies-schema.json\",\n  \"title\": \"Policies\",\n  \"description\": \"Policies schema from Apache Pulsar\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"replication_clusters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"bundles\": {\n      \"type\": \"object\"\n    },\n    \"retention_policies\": {\n      \"$ref\": \"#/components/schemas/RetentionPolicies\"\n    },\n    \"schema_auto_update_compatibility_strategy\": {\n      \"type\": \"string\"\n    },\n    \"message_ttl_in_seconds\": {\n      \"type\": \"integer\"\n    },\n    \"max_producers_per_topic\": {\n      \"type\": \"integer\"\n    },\n    \"max_consumers_per_topic\": {\n      \"type\": \"integer\"\n    },\n    \"max_consumers_per_subscription\": {\n      \"\
  type\": \"integer\"\n    },\n    \"backlog_quota_map\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-policies-schema.json
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: Policies
---
