---
description: Represents a snapshot of a streaming Dataflow job. A snapshot captures the state of the pipeline at a point in time and can be used to start a new job from that state.
layout: schema
name: Google Cloud Dataflow Snapshot
properties_list:
- description: The unique identifier of the snapshot.
  name: id
  type: string
- description: The project this snapshot belongs to.
  name: projectId
  type: string
- description: The job from which this snapshot was created.
  name: sourceJobId
  type: string
- description: The time this snapshot was created.
  name: creationTime
  type: string
- description: 'The time-to-live duration for the snapshot, after which it will be automatically deleted. Format: a duration string such as 3600s.'
  name: ttl
  type: string
- description: The current state of the snapshot.
  name: state
  type: string
- description: User-specified description of the snapshot.
  name: description
  type: string
- description: Pub/Sub snapshot metadata associated with this Dataflow snapshot.
  name: pubsubMetadata
  type: array
- description: The disk byte size of the snapshot.
  name: diskSizeBytes
  type: string
- description: The Cloud region where this snapshot resides, such as us-central1.
  name: region
  type: string
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
schema_file: json-schema/google-cloud-dataflow-snapshot-schema.json
slug: google-cloud-dataflow-snapshot
source_filename: google-cloud-dataflow-snapshot-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/google-cloud-dataflow/json-schema/google-cloud-dataflow-snapshot-schema.json\",\n  \"title\": \"Google Cloud Dataflow Snapshot\",\n  \"description\": \"Represents a snapshot of a streaming Dataflow job. A snapshot captures the state of the pipeline at a point in time and can be used to start a new job from that state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the snapshot.\",\n      \"readOnly\": true\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The project this snapshot belongs to.\"\n    },\n    \"sourceJobId\": {\n      \"type\": \"string\",\n      \"description\": \"The job from which this snapshot was created.\"\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The time this snapshot was created.\",\n      \"readOnly\": true\n    },\n    \"ttl\": {\n      \"type\": \"string\",\n      \"description\": \"The time-to-live duration for the snapshot, after which it will be automatically deleted. Format: a duration string such as 3600s.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the snapshot.\",\n      \"enum\": [\n        \"UNKNOWN_SNAPSHOT_STATE\",\n        \"PENDING\",\n        \"RUNNING\",\n        \"READY\",\n        \"FAILED\",\n        \"DELETED\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-specified description of the snapshot.\"\n    },\n    \"pubsubMetadata\": {\n      \"type\": \"array\",\n      \"description\": \"Pub/Sub snapshot metadata associated with this Dataflow snapshot.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"topicName\": {\n            \"type\": \"string\"\
  ,\n            \"description\": \"The name of the Pub/Sub topic.\"\n          },\n          \"snapshotName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the Pub/Sub snapshot.\"\n          },\n          \"expireTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The expire time of the Pub/Sub snapshot.\"\n          }\n        }\n      }\n    },\n    \"diskSizeBytes\": {\n      \"type\": \"string\",\n      \"format\": \"int64\",\n      \"description\": \"The disk byte size of the snapshot.\",\n      \"readOnly\": true\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The Cloud region where this snapshot resides, such as us-central1.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/json-schema/google-cloud-dataflow-snapshot-schema.json
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
title: Google Cloud Dataflow Snapshot
---
