---
description: JSON Schema for Resilience4j bulkhead and thread pool bulkhead configuration properties.
layout: schema
name: Resilience4j Bulkhead Configuration
properties_list:
- description: ''
  name: resilience4j
  type: object
provider_name: Resilience4j
provider_slug: resilience4j
schema_file: json-schema/bulkhead-configuration.json
slug: bulkhead-configuration
source_filename: bulkhead-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resilience4j/json-schema/bulkhead-configuration.json\",\n  \"title\": \"Resilience4j Bulkhead Configuration\",\n  \"description\": \"JSON Schema for Resilience4j bulkhead and thread pool bulkhead configuration properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resilience4j\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"bulkhead\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"configs\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/BulkheadConfig\"\n              }\n            },\n            \"instances\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/BulkheadInstance\"\n              }\n            }\n          }\n        },\n        \"thread-pool-bulkhead\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"configs\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/ThreadPoolBulkheadConfig\"\n              }\n            },\n            \"instances\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/ThreadPoolBulkheadInstance\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"BulkheadConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"maxConcurrentCalls\": {\n          \"type\": \"integer\",\n          \"default\": 25,\n          \"description\": \"Maximum number of concurrent calls allowed.\"\n        },\n        \"maxWaitDuration\": {\n          \"type\": \"string\",\n          \"default\": \"0ms\",\n          \"description\": \"Maximum wait duration for a call to acquire permission.\"\n     \
  \   },\n        \"writableStackTraceEnabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether BulkheadFullException has a writable stack trace.\"\n        }\n      }\n    },\n    \"BulkheadInstance\": {\n      \"allOf\": [\n        { \"$ref\": \"#/$defs/BulkheadConfig\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"baseConfig\": {\n              \"type\": \"string\",\n              \"description\": \"Name of a shared configuration to inherit from.\"\n            }\n          }\n        }\n      ]\n    },\n    \"ThreadPoolBulkheadConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"maxThreadPoolSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum thread pool size.\"\n        },\n        \"coreThreadPoolSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Core thread pool size.\"\n        },\n        \"queueCapacity\"\
  : {\n          \"type\": \"integer\",\n          \"default\": 100,\n          \"description\": \"Capacity of the queue.\"\n        },\n        \"keepAliveDuration\": {\n          \"type\": \"string\",\n          \"default\": \"20ms\",\n          \"description\": \"Duration for which excess threads stay alive.\"\n        },\n        \"writableStackTraceEnabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether BulkheadFullException has a writable stack trace.\"\n        }\n      }\n    },\n    \"ThreadPoolBulkheadInstance\": {\n      \"allOf\": [\n        { \"$ref\": \"#/$defs/ThreadPoolBulkheadConfig\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"baseConfig\": {\n              \"type\": \"string\",\n              \"description\": \"Name of a shared configuration to inherit from.\"\n            }\n          }\n        }\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resilience4j/refs/heads/main/json-schema/bulkhead-configuration.json
tags:
- Bulkhead
- Circuit Breaker
- Fault Tolerance
- Java
- Microservices
- Rate Limiter
- Resilience
- Retry
- Spring Boot
- Functional Programming
title: Resilience4j Bulkhead Configuration
---
