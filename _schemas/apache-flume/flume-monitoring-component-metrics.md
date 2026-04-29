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
source_filename: flume-monitoring-component-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flume/refs/heads/main/json-schema/flume-monitoring-component-metrics-schema.json\",\n  \"title\": \"ComponentMetrics\",\n  \"description\": \"Metrics for a specific Flume component (source, channel, or sink)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"Component type (SOURCE, CHANNEL, or SINK)\",\n      \"enum\": [\n        \"SOURCE\",\n        \"CHANNEL\",\n        \"SINK\"\n      ],\n      \"example\": \"SOURCE\"\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"description\": \"Component start timestamp in milliseconds since epoch\",\n      \"example\": \"1718153645993\"\n    },\n    \"StopTime\": {\n      \"type\": \"string\",\n      \"description\": \"Component stop timestamp (0 if running)\",\n      \"example\": \"0\"\n    },\n    \"EventReceivedCount\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Number of events received (sources only)\",\n      \"example\": \"1000\"\n    },\n    \"EventAcceptedCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of events accepted (sources only)\",\n      \"example\": \"998\"\n    },\n    \"AppendBatchReceivedCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of event batches received (sources only)\",\n      \"example\": \"50\"\n    },\n    \"AppendBatchAcceptedCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of event batches accepted (sources only)\",\n      \"example\": \"50\"\n    },\n    \"EventPutAttemptCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of event put attempts (channels only)\",\n      \"example\": \"998\"\n    },\n    \"EventPutSuccessCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of successful event puts (channels only)\",\n      \"example\": \"998\"\
  \n    },\n    \"EventTakeAttemptCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of event take attempts (channels only)\",\n      \"example\": \"998\"\n    },\n    \"EventTakeSuccessCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of successful event takes (channels only)\",\n      \"example\": \"997\"\n    },\n    \"ChannelSize\": {\n      \"type\": \"string\",\n      \"description\": \"Current number of events in channel\",\n      \"example\": \"1\"\n    },\n    \"ChannelCapacity\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum channel capacity in events\",\n      \"example\": \"1000\"\n    },\n    \"EventDrainAttemptCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of drain attempts (sinks only)\",\n      \"example\": \"997\"\n    },\n    \"EventDrainSuccessCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of successful drains (sinks only)\",\n      \"example\": \"997\"\n\
  \    },\n    \"ConnectionCreatedCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of connections created (sinks only)\",\n      \"example\": \"5\"\n    },\n    \"ConnectionClosedCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of connections closed (sinks only)\",\n      \"example\": \"4\"\n    },\n    \"ConnectionFailedCount\": {\n      \"type\": \"string\",\n      \"description\": \"Number of failed connections (sinks only)\",\n      \"example\": \"0\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flume/refs/heads/main/json-schema/flume-monitoring-component-metrics-schema.json
tags:
- Apache
- Data Collection
- ETL
- Log Aggregation
- Open Source
- Streaming
title: ComponentMetrics
---
