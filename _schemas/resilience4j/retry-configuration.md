---
description: JSON Schema for Resilience4j retry configuration properties.
layout: schema
name: Resilience4j Retry Configuration
properties_list:
- description: ''
  name: resilience4j
  type: object
provider_name: Resilience4j
provider_slug: resilience4j
schema_file: json-schema/retry-configuration.json
slug: retry-configuration
source_filename: retry-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resilience4j/json-schema/retry-configuration.json\",\n  \"title\": \"Resilience4j Retry Configuration\",\n  \"description\": \"JSON Schema for Resilience4j retry configuration properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resilience4j\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"retry\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"configs\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/RetryConfig\"\n              }\n            },\n            \"instances\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"$ref\": \"#/$defs/RetryInstance\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"RetryConfig\": {\n\
  \      \"type\": \"object\",\n      \"properties\": {\n        \"maxAttempts\": {\n          \"type\": \"integer\",\n          \"default\": 3,\n          \"description\": \"Maximum number of retry attempts.\"\n        },\n        \"waitDuration\": {\n          \"type\": \"string\",\n          \"default\": \"500ms\",\n          \"description\": \"Fixed wait duration between retry attempts.\"\n        },\n        \"enableExponentialBackoff\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether exponential backoff is enabled.\"\n        },\n        \"exponentialBackoffMultiplier\": {\n          \"type\": \"number\",\n          \"default\": 2,\n          \"description\": \"Multiplier for exponential backoff.\"\n        },\n        \"enableRandomizedWait\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether randomized wait is enabled.\"\n        },\n        \"randomizedWaitFactor\": {\n\
  \          \"type\": \"number\",\n          \"default\": 0.5,\n          \"description\": \"Randomization factor for wait duration.\"\n        },\n        \"retryExceptions\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"List of exception class names that trigger a retry.\"\n        },\n        \"ignoreExceptions\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"List of exception class names that are ignored.\"\n        },\n        \"failAfterMaxAttempts\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether to throw MaxRetriesExceededException after all attempts.\"\n        }\n      }\n    },\n    \"RetryInstance\": {\n      \"allOf\": [\n        { \"$ref\": \"#/$defs/RetryConfig\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"baseConfig\": {\n              \"\
  type\": \"string\",\n              \"description\": \"Name of a shared configuration to inherit from.\"\n            }\n          }\n        }\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resilience4j/refs/heads/main/json-schema/retry-configuration.json
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
title: Resilience4j Retry Configuration
---
