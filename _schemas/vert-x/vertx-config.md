---
description: JSON Schema for Vert.x application configuration options including event bus, cluster, HTTP server, and deployment settings.
layout: schema
name: Vert.x Application Configuration
properties_list:
- description: HTTP server configuration.
  name: http
  type: object
- description: Event bus configuration for clustered and local mode.
  name: eventBus
  type: object
- description: Cluster manager settings.
  name: cluster
  type: object
- description: Maximum number of worker threads.
  name: workerPoolSize
  type: integer
- description: Number of event loop threads.
  name: eventLoopPoolSize
  type: integer
- description: Size of the internal blocking pool.
  name: internalBlockingPoolSize
  type: integer
- description: Enable high availability.
  name: haEnabled
  type: boolean
- description: High availability group name.
  name: haGroup
  type: string
- description: Quorum size for HA.
  name: quorumSize
  type: integer
- description: Blocked thread check interval in milliseconds.
  name: blockedThreadCheckInterval
  type: integer
- description: Max event loop execute time in nanoseconds.
  name: maxEventLoopExecuteTime
  type: integer
- description: Max worker execute time in nanoseconds.
  name: maxWorkerExecuteTime
  type: integer
- description: Warning exception time in nanoseconds.
  name: warningExceptionTime
  type: integer
provider_name: Vert.x
provider_slug: vert-x
schema_file: json-schema/vertx-config.json
slug: vertx-config
source_filename: vertx-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vert-x/json-schema/vertx-config.json\",\n  \"title\": \"Vert.x Application Configuration\",\n  \"description\": \"JSON Schema for Vert.x application configuration options including event bus, cluster, HTTP server, and deployment settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"http\": {\n      \"type\": \"object\",\n      \"description\": \"HTTP server configuration.\",\n      \"properties\": {\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port the HTTP server listens on.\",\n          \"default\": 8080,\n          \"minimum\": 0,\n          \"maximum\": 65535\n        },\n        \"host\": {\n          \"type\": \"string\",\n          \"description\": \"The host address to bind.\",\n          \"default\": \"0.0.0.0\"\n        },\n        \"ssl\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Enable SSL/TLS.\",\n          \"default\": false\n        },\n        \"keyStorePath\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the key store for SSL.\"\n        },\n        \"keyStorePassword\": {\n          \"type\": \"string\",\n          \"description\": \"Password for the key store.\"\n        },\n        \"compressionSupported\": {\n          \"type\": \"boolean\",\n          \"description\": \"Enable HTTP compression.\",\n          \"default\": false\n        },\n        \"idleTimeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Idle timeout in seconds.\",\n          \"default\": 0\n        },\n        \"maxWebSocketFrameSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum WebSocket frame size in bytes.\",\n          \"default\": 65536\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"eventBus\": {\n      \"type\": \"object\",\n      \"description\": \"Event bus configuration\
  \ for clustered and local mode.\",\n      \"properties\": {\n        \"clusterPublicHost\": {\n          \"type\": \"string\",\n          \"description\": \"Public host address for cluster event bus.\"\n        },\n        \"clusterPublicPort\": {\n          \"type\": \"integer\",\n          \"description\": \"Public port for cluster event bus.\",\n          \"minimum\": 0,\n          \"maximum\": 65535\n        },\n        \"clusterPingInterval\": {\n          \"type\": \"integer\",\n          \"description\": \"Cluster ping interval in milliseconds.\",\n          \"default\": 20000\n        },\n        \"clusterPingReplyInterval\": {\n          \"type\": \"integer\",\n          \"description\": \"Cluster ping reply interval in milliseconds.\",\n          \"default\": 20000\n        },\n        \"connectTimeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Event bus connect timeout in milliseconds.\",\n          \"default\": 60000\n        }\n      },\n      \"\
  additionalProperties\": true\n    },\n    \"cluster\": {\n      \"type\": \"object\",\n      \"description\": \"Cluster manager settings.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Enable clustering.\",\n          \"default\": false\n        },\n        \"clusterManager\": {\n          \"type\": \"string\",\n          \"description\": \"Fully qualified class name of the cluster manager implementation.\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"workerPoolSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of worker threads.\",\n      \"default\": 20,\n      \"minimum\": 1\n    },\n    \"eventLoopPoolSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of event loop threads.\",\n      \"minimum\": 1\n    },\n    \"internalBlockingPoolSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the internal blocking pool.\"\
  ,\n      \"default\": 20,\n      \"minimum\": 1\n    },\n    \"haEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable high availability.\",\n      \"default\": false\n    },\n    \"haGroup\": {\n      \"type\": \"string\",\n      \"description\": \"High availability group name.\",\n      \"default\": \"__DEFAULT__\"\n    },\n    \"quorumSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Quorum size for HA.\",\n      \"default\": 1,\n      \"minimum\": 1\n    },\n    \"blockedThreadCheckInterval\": {\n      \"type\": \"integer\",\n      \"description\": \"Blocked thread check interval in milliseconds.\",\n      \"default\": 1000\n    },\n    \"maxEventLoopExecuteTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Max event loop execute time in nanoseconds.\",\n      \"default\": 2000000000\n    },\n    \"maxWorkerExecuteTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Max worker execute time in nanoseconds.\",\n      \"\
  default\": 60000000000\n    },\n    \"warningExceptionTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Warning exception time in nanoseconds.\",\n      \"default\": 5000000000\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vert-x/refs/heads/main/json-schema/vertx-config.json
tags:
- Event-Driven
- Frameworks
- Java
- JVM
- Microservices
- Polyglot
- Reactive
title: Vert.x Application Configuration
---
