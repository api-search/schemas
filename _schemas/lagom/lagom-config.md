---
description: JSON Schema representing the Lagom framework configuration structure (application.conf in HOCON format) covering service locator, persistence, clustering, and broker settings.
layout: schema
name: Lagom Application Configuration
properties_list:
- description: ''
  name: lagom
  type: object
provider_name: Lagom
provider_slug: lagom
schema_file: json-schema/lagom-config.json
slug: lagom-config
source_filename: lagom-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/lagom/json-schema/lagom-config.json\",\n  \"title\": \"Lagom Application Configuration\",\n  \"description\": \"JSON Schema representing the Lagom framework configuration structure (application.conf in HOCON format) covering service locator, persistence, clustering, and broker settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lagom\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"services\": {\n          \"type\": \"object\",\n          \"description\": \"Service locator configuration for locating other services.\",\n          \"additionalProperties\": {\n            \"type\": \"string\",\n            \"description\": \"URI of the service.\"\n          }\n        },\n        \"persistence\": {\n          \"type\": \"object\",\n          \"description\": \"Persistence and read-side configuration.\",\n          \"properties\"\
  : {\n            \"maxNumberOfShards\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of shards for persistent entity distribution.\",\n              \"default\": 100\n            },\n            \"snapshotAfter\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of events before taking a snapshot.\",\n              \"default\": 100\n            },\n            \"askTimeout\": {\n              \"type\": \"string\",\n              \"description\": \"Timeout for asks to persistent entities.\",\n              \"default\": \"5s\"\n            },\n            \"readSide\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"cassandra\": {\n                  \"type\": \"object\",\n                  \"description\": \"Cassandra read-side processor settings.\",\n                  \"properties\": {\n                    \"keyspace\": {\n                      \"type\": \"string\"\n          \
  \          }\n                  },\n                  \"additionalProperties\": true\n                }\n              },\n              \"additionalProperties\": true\n            }\n          },\n          \"additionalProperties\": true\n        },\n        \"broker\": {\n          \"type\": \"object\",\n          \"description\": \"Message broker configuration.\",\n          \"properties\": {\n            \"kafka\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"serviceNamePrefix\": {\n                  \"type\": \"string\",\n                  \"description\": \"Prefix for Kafka service name.\",\n                  \"default\": \"kafka_native\"\n                },\n                \"brokers\": {\n                  \"type\": \"string\",\n                  \"description\": \"Comma-separated list of Kafka broker addresses.\"\n                }\n              },\n              \"additionalProperties\": true\n            }\n          },\n      \
  \    \"additionalProperties\": true\n        },\n        \"cluster\": {\n          \"type\": \"object\",\n          \"description\": \"Akka Cluster settings for Lagom.\",\n          \"properties\": {\n            \"joinSelf\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the node should join itself to form a cluster.\",\n              \"default\": true\n            },\n            \"exitJvm\": {\n              \"type\": \"boolean\",\n              \"description\": \"Exit the JVM on ActorSystem termination.\",\n              \"default\": true\n            }\n          },\n          \"additionalProperties\": true\n        },\n        \"circuitBreaker\": {\n          \"type\": \"object\",\n          \"description\": \"Default circuit breaker configuration.\",\n          \"properties\": {\n            \"default\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"enabled\": {\n                  \"type\": \"boolean\"\
  ,\n                  \"default\": true\n                },\n                \"maxFailures\": {\n                  \"type\": \"integer\",\n                  \"default\": 10\n                },\n                \"callTimeout\": {\n                  \"type\": \"string\",\n                  \"default\": \"10s\"\n                },\n                \"resetTimeout\": {\n                  \"type\": \"string\",\n                  \"default\": \"15s\"\n                }\n              },\n              \"additionalProperties\": true\n            }\n          },\n          \"additionalProperties\": true\n        }\n      },\n      \"additionalProperties\": true\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lagom/refs/heads/main/json-schema/lagom-config.json
tags:
- Akka
- Event Sourcing
- Frameworks
- Java
- Microservices
- Reactive
- Scala
title: Lagom Application Configuration
---
