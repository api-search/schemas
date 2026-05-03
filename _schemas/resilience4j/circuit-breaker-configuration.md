---
description: JSON Schema for Resilience4j circuit breaker configuration properties used in application.yml or application.properties.
layout: schema
name: Resilience4j Circuit Breaker Configuration
properties_list:
- description: ''
  name: resilience4j
  type: object
provider_name: Resilience4j
provider_slug: resilience4j
schema_file: json-schema/circuit-breaker-configuration.json
slug: circuit-breaker-configuration
source_filename: circuit-breaker-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resilience4j/json-schema/circuit-breaker-configuration.json\",\n  \"title\": \"Resilience4j Circuit Breaker Configuration\",\n  \"description\": \"JSON Schema for Resilience4j circuit breaker configuration properties used in application.yml or application.properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resilience4j\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"circuitbreaker\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"configs\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/CircuitBreakerConfig\"\n              }\n            },\n            \"instances\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/CircuitBreakerInstance\"\n        \
  \      }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"CircuitBreakerConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"slidingWindowType\": {\n          \"type\": \"string\",\n          \"enum\": [\"COUNT_BASED\", \"TIME_BASED\"],\n          \"default\": \"COUNT_BASED\",\n          \"description\": \"Type of sliding window used to record calls.\"\n        },\n        \"slidingWindowSize\": {\n          \"type\": \"integer\",\n          \"default\": 100,\n          \"description\": \"Size of the sliding window.\"\n        },\n        \"minimumNumberOfCalls\": {\n          \"type\": \"integer\",\n          \"default\": 100,\n          \"description\": \"Minimum number of calls before the circuit breaker can calculate the error rate.\"\n        },\n        \"failureRateThreshold\": {\n          \"type\": \"number\",\n          \"default\": 50,\n          \"description\": \"Failure rate threshold in percentage above which the\
  \ circuit breaker opens.\"\n        },\n        \"slowCallRateThreshold\": {\n          \"type\": \"number\",\n          \"default\": 100,\n          \"description\": \"Slow call rate threshold in percentage.\"\n        },\n        \"slowCallDurationThreshold\": {\n          \"type\": \"string\",\n          \"default\": \"60s\",\n          \"description\": \"Duration threshold above which a call is considered slow.\"\n        },\n        \"waitDurationInOpenState\": {\n          \"type\": \"string\",\n          \"default\": \"60s\",\n          \"description\": \"Duration the circuit breaker stays open before transitioning to half-open.\"\n        },\n        \"permittedNumberOfCallsInHalfOpenState\": {\n          \"type\": \"integer\",\n          \"default\": 10,\n          \"description\": \"Number of permitted calls in half-open state.\"\n        },\n        \"automaticTransitionFromOpenToHalfOpenEnabled\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n        \
  \  \"description\": \"Whether to automatically transition from open to half-open.\"\n        },\n        \"recordExceptions\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"List of exception class names that are recorded as failures.\"\n        },\n        \"ignoreExceptions\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"List of exception class names that are ignored.\"\n        },\n        \"writableStackTraceEnabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether CallNotPermittedException has a writable stack trace.\"\n        }\n      }\n    },\n    \"CircuitBreakerInstance\": {\n      \"allOf\": [\n        { \"$ref\": \"#/$defs/CircuitBreakerConfig\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"baseConfig\": {\n              \"type\": \"string\",\n\
  \              \"description\": \"Name of a shared configuration to inherit from.\"\n            }\n          }\n        }\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resilience4j/refs/heads/main/json-schema/circuit-breaker-configuration.json
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
title: Resilience4j Circuit Breaker Configuration
---
