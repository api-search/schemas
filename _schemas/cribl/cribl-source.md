---
description: A Cribl data input source that collects events from various systems and protocols for processing through pipelines and delivery to destinations.
layout: schema
name: Cribl Source
properties_list:
- description: Unique identifier for the source
  name: id
  type: string
- description: The source type that determines the collection protocol and configuration options
  name: type
  type: string
- description: Whether the source is disabled and not actively collecting data
  name: disabled
  type: boolean
- description: The host or IP address to listen on for network-based sources
  name: host
  type: string
- description: The port number to listen on for network-based sources
  name: port
  type: integer
- description: ''
  name: tls
  type: object
- description: The authentication method required for incoming connections
  name: authType
  type: string
- description: The authentication token required for token-based authentication
  name: authToken
  type: string
- description: The pipeline identifier to route events from this source to
  name: pipeline
  type: string
- description: A human-readable description of the source purpose
  name: description
  type: string
- description: The environment context tag applied to events from this source
  name: environment
  type: string
- description: Tags applied to all events collected from this source
  name: streamtags
  type: array
- description: Maximum number of concurrent connections for network sources
  name: maxConnections
  type: integer
- description: Whether to honor proxy protocol headers
  name: enableProxyHeader
  type: boolean
provider_name: Cribl
provider_slug: cribl
schema_file: json-schema/cribl-source-schema.json
slug: cribl-source
source_filename: cribl-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.cribl.io/schemas/cribl/source.json\",\n  \"title\": \"Cribl Source\",\n  \"description\": \"A Cribl data input source that collects events from various systems and protocols for processing through pipelines and delivery to destinations.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the source\",\n      \"pattern\": \"^[a-zA-Z0-9_:-]+$\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The source type that determines the collection protocol and configuration options\",\n      \"enum\": [\n        \"syslog\",\n        \"http\",\n        \"splunk_tcp\",\n        \"splunk_hec\",\n        \"tcp_json\",\n        \"kafka\",\n        \"kinesis\",\n        \"s3\",\n        \"sqs\",\n        \"azure_blob\",\n        \"azure_event_hub\"\
  ,\n        \"google_cloud_pubsub\",\n        \"file_monitor\",\n        \"windows_event_log\",\n        \"system_metrics\",\n        \"appscope\",\n        \"journald\",\n        \"cribl_http\",\n        \"cribl_tcp\",\n        \"snmp\",\n        \"graphite\",\n        \"statsd\",\n        \"collectd\",\n        \"elastic\"\n      ]\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the source is disabled and not actively collecting data\",\n      \"default\": false\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The host or IP address to listen on for network-based sources\",\n      \"format\": \"hostname\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number to listen on for network-based sources\",\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"tls\": {\n      \"$ref\": \"#/$defs/TlsConfig\"\n    },\n    \"authType\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The authentication method required for incoming connections\",\n      \"enum\": [\n        \"none\",\n        \"token\",\n        \"basic\",\n        \"mutual_tls\"\n      ]\n    },\n    \"authToken\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication token required for token-based authentication\"\n    },\n    \"pipeline\": {\n      \"type\": \"string\",\n      \"description\": \"The pipeline identifier to route events from this source to\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the source purpose\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"The environment context tag applied to events from this source\"\n    },\n    \"streamtags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to all events collected from this source\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n\
  \    \"maxConnections\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of concurrent connections for network sources\",\n      \"minimum\": 1\n    },\n    \"enableProxyHeader\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to honor proxy protocol headers\",\n      \"default\": false\n    }\n  },\n  \"$defs\": {\n    \"TlsConfig\": {\n      \"type\": \"object\",\n      \"description\": \"TLS/SSL configuration for encrypted connections.\",\n      \"properties\": {\n        \"disabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether TLS is disabled\",\n          \"default\": true\n        },\n        \"certPath\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the TLS certificate file\"\n        },\n        \"privKeyPath\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the TLS private key file\"\n        },\n        \"caPath\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Path to the CA certificate for client verification\"\n        },\n        \"minVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum TLS version to accept\",\n          \"enum\": [\"TLSv1\", \"TLSv1.1\", \"TLSv1.2\", \"TLSv1.3\"],\n          \"default\": \"TLSv1.2\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cribl/refs/heads/main/json-schema/cribl-source-schema.json
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
title: Cribl Source
---
