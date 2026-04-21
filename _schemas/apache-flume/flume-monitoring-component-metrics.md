---
description: Metrics for a specific Flume component (source, channel, or sink)
layout: schema
name: ComponentMetrics
properties_list:
- description: Component type (SOURCE, CHANNEL, or SINK)
  name: Type
  type: string
- description: Component start timestamp in milliseconds since epoch
  name: StartTime
  type: string
- description: Component stop timestamp (0 if running)
  name: StopTime
  type: string
- description: Number of events received (sources only)
  name: EventReceivedCount
  type: string
- description: Number of events accepted (sources only)
  name: EventAcceptedCount
  type: string
- description: Number of event batches received (sources only)
  name: AppendBatchReceivedCount
  type: string
- description: Number of event batches accepted (sources only)
  name: AppendBatchAcceptedCount
  type: string
- description: Number of event put attempts (channels only)
  name: EventPutAttemptCount
  type: string
- description: Number of successful event puts (channels only)
  name: EventPutSuccessCount
  type: string
- description: Number of event take attempts (channels only)
  name: EventTakeAttemptCount
  type: string
- description: Number of successful event takes (channels only)
  name: EventTakeSuccessCount
  type: string
- description: Current number of events in channel
  name: ChannelSize
  type: string
- description: Maximum channel capacity in events
  name: ChannelCapacity
  type: string
- description: Number of drain attempts (sinks only)
  name: EventDrainAttemptCount
  type: string
- description: Number of successful drains (sinks only)
  name: EventDrainSuccessCount
  type: string
- description: Number of connections created (sinks only)
  name: ConnectionCreatedCount
  type: string
- description: Number of connections closed (sinks only)
  name: ConnectionClosedCount
  type: string
- description: Number of failed connections (sinks only)
  name: ConnectionFailedCount
  type: string
provider_name: Apache Flume
provider_slug: apache-flume
schema_file: json-schema/flume-monitoring-component-metrics-schema.json
slug: flume-monitoring-component-metrics
tags:
- Apache
- Data Collection
- ETL
- Log Aggregation
- Open Source
- Streaming
title: ComponentMetrics
---
