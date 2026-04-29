---
description: A Cribl data output destination that receives processed events from pipelines and delivers them to analytics platforms, storage systems, and other downstream targets.
layout: schema
name: Cribl Destination
properties_list:
- description: Unique identifier for the destination
  name: id
  type: string
- description: The destination type that determines the delivery protocol and configuration options
  name: type
  type: string
- description: Whether the destination is disabled
  name: disabled
  type: boolean
- description: The target host address for the destination
  name: host
  type: string
- description: The target port number
  name: port
  type: integer
- description: TLS/SSL configuration for encrypted delivery
  name: tls
  type: object
- description: A human-readable description of the destination purpose
  name: description
  type: string
- description: The environment context tag for this destination
  name: environment
  type: string
- description: Tags used for filtering events to this destination
  name: streamtags
  type: array
- description: Maximum events per second to send to this destination
  name: throttleRatePerSec
  type: integer
- description: Behavior when the destination cannot keep up with incoming events
  name: onBackpressure
  type: string
- description: ''
  name: pq
  type: object
provider_name: Cribl
provider_slug: cribl
schema_file: json-schema/cribl-destination-schema.json
slug: cribl-destination
source_filename: cribl-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.cribl.io/schemas/cribl/destination.json\",\n  \"title\": \"Cribl Destination\",\n  \"description\": \"A Cribl data output destination that receives processed events from pipelines and delivers them to analytics platforms, storage systems, and other downstream targets.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the destination\",\n      \"pattern\": \"^[a-zA-Z0-9_:-]+$\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The destination type that determines the delivery protocol and configuration options\",\n      \"enum\": [\n        \"splunk\",\n        \"splunk_hec\",\n        \"s3\",\n        \"elasticsearch\",\n        \"kafka\",\n        \"kinesis\",\n        \"syslog\",\n        \"tcp_json\",\n        \"webhook\"\
  ,\n        \"azure_blob\",\n        \"azure_event_hub\",\n        \"azure_monitor\",\n        \"google_cloud_storage\",\n        \"google_cloud_pubsub\",\n        \"google_chronicle\",\n        \"datadog\",\n        \"new_relic\",\n        \"sumo_logic\",\n        \"cribl_lake\",\n        \"cribl_http\",\n        \"filesystem\",\n        \"devnull\",\n        \"default\",\n        \"graphite\",\n        \"statsd\",\n        \"honeycomb\",\n        \"loki\",\n        \"minio\",\n        \"snowflake\"\n      ]\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the destination is disabled\",\n      \"default\": false\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The target host address for the destination\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The target port number\",\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"tls\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"TLS/SSL configuration for encrypted delivery\",\n      \"properties\": {\n        \"disabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether TLS is disabled\",\n          \"default\": true\n        },\n        \"certPath\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the TLS certificate file\"\n        },\n        \"privKeyPath\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the TLS private key file\"\n        },\n        \"caPath\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the CA certificate for server verification\"\n        },\n        \"rejectUnauthorized\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to reject connections with invalid certificates\",\n          \"default\": true\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description\
  \ of the destination purpose\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"The environment context tag for this destination\"\n    },\n    \"streamtags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags used for filtering events to this destination\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"throttleRatePerSec\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum events per second to send to this destination\",\n      \"minimum\": 0\n    },\n    \"onBackpressure\": {\n      \"type\": \"string\",\n      \"description\": \"Behavior when the destination cannot keep up with incoming events\",\n      \"enum\": [\n        \"drop\",\n        \"block\",\n        \"queue\"\n      ]\n    },\n    \"pq\": {\n      \"$ref\": \"#/$defs/PersistentQueue\"\n    }\n  },\n  \"$defs\": {\n    \"PersistentQueue\": {\n      \"type\": \"object\",\n      \"description\": \"Persistent queue configuration for\
  \ buffering events during destination outages.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether persistent queuing is enabled\",\n          \"default\": false\n        },\n        \"maxSize\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum queue size with unit suffix such as 1GB, 500MB\",\n          \"pattern\": \"^[0-9]+(GB|MB|KB)$\"\n        },\n        \"maxEvents\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of events to queue\",\n          \"minimum\": 0\n        },\n        \"compress\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to compress queued data\",\n          \"default\": false\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/json-schema/cribl-destination-schema.json
tags:
- Configuration
- Data Lake
- Data Pipelines
- Data Routing
- Edge Computing
- Infrastructure as Code
- Observability
- Search
- Security Data
- Stream Processing
- Telemetry
title: Cribl Destination
---
