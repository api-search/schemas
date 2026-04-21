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
