---
description: Represents a Datastream stream, which defines the configuration for replicating data from a source to a destination.
layout: schema
name: Google Cloud Datastream Stream
properties_list:
- description: Output only. The resource name of the stream.
  name: name
  type: string
- description: Output only. The creation time of the stream.
  name: createTime
  type: string
- description: Output only. The last update time of the stream.
  name: updateTime
  type: string
- description: Labels for the stream.
  name: labels
  type: object
- description: Display name for the stream.
  name: displayName
  type: string
- description: Source connection profile configuration.
  name: sourceConfig
  type: object
- description: Destination connection profile configuration.
  name: destinationConfig
  type: object
- description: The state of the stream.
  name: state
  type: string
- description: Output only. Errors on the stream.
  name: errors
  type: array
provider_name: Google Cloud Datastream
provider_slug: google-cloud-datastream
schema_file: json-schema/google-cloud-datastream-stream-schema.json
slug: google-cloud-datastream-stream
source_filename: google-cloud-datastream-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-datastream/refs/heads/main/json-schema/google-cloud-datastream-stream-schema.json\",\n  \"title\": \"Google Cloud Datastream Stream\",\n  \"description\": \"Represents a Datastream stream, which defines the configuration for replicating data from a source to a destination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The resource name of the stream.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. The creation time of the stream.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. The last update time of the stream.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n    \
  \  \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels for the stream.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the stream.\"\n    },\n    \"sourceConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Source connection profile configuration.\",\n      \"properties\": {\n        \"sourceConnectionProfile\": {\n          \"type\": \"string\",\n          \"description\": \"The resource name of the source connection profile.\"\n        },\n        \"oracleSourceConfig\": {\n          \"type\": \"object\",\n          \"description\": \"Oracle source configuration.\"\n        },\n        \"mysqlSourceConfig\": {\n          \"type\": \"object\",\n          \"description\": \"MySQL source configuration.\"\n        },\n        \"postgresqlSourceConfig\": {\n          \"type\": \"object\",\n          \"description\": \"PostgreSQL source configuration.\"\n        }\n    \
  \  },\n      \"required\": [\"sourceConnectionProfile\"]\n    },\n    \"destinationConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Destination connection profile configuration.\",\n      \"properties\": {\n        \"destinationConnectionProfile\": {\n          \"type\": \"string\",\n          \"description\": \"The resource name of the destination connection profile.\"\n        },\n        \"gcsDestinationConfig\": {\n          \"type\": \"object\",\n          \"description\": \"Cloud Storage destination configuration.\",\n          \"properties\": {\n            \"path\": { \"type\": \"string\" },\n            \"fileRotationMb\": { \"type\": \"integer\" },\n            \"fileRotationInterval\": { \"type\": \"string\" }\n          }\n        },\n        \"bigqueryDestinationConfig\": {\n          \"type\": \"object\",\n          \"description\": \"BigQuery destination configuration.\"\n        }\n      },\n      \"required\": [\"destinationConnectionProfile\"]\n    },\n\
  \    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"STATE_UNSPECIFIED\",\n        \"NOT_STARTED\",\n        \"RUNNING\",\n        \"PAUSED\",\n        \"MAINTENANCE\",\n        \"FAILED\",\n        \"FAILED_PERMANENTLY\",\n        \"STARTING\",\n        \"DRAINING\"\n      ],\n      \"description\": \"The state of the stream.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Output only. Errors on the stream.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"reason\": { \"type\": \"string\" },\n          \"errorUuid\": { \"type\": \"string\" },\n          \"message\": { \"type\": \"string\" },\n          \"errorTime\": { \"type\": \"string\", \"format\": \"date-time\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"displayName\", \"sourceConfig\", \"destinationConfig\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-datastream/refs/heads/main/json-schema/google-cloud-datastream-stream-schema.json
tags:
- Change Data Capture
- Data Replication
- Google Cloud
- Streaming
title: Google Cloud Datastream Stream
---
