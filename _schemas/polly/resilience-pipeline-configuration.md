---
description: JSON Schema for Polly v8+ resilience pipeline configuration used in .NET applications with Microsoft.Extensions.Resilience.
layout: schema
name: Polly Resilience Pipeline Configuration
properties_list:
- description: Named resilience pipeline configurations.
  name: ResiliencePipelines
  type: object
provider_name: Polly
provider_slug: polly
schema_file: json-schema/resilience-pipeline-configuration.json
slug: resilience-pipeline-configuration
source_filename: resilience-pipeline-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polly/json-schema/resilience-pipeline-configuration.json\",\n  \"title\": \"Polly Resilience Pipeline Configuration\",\n  \"description\": \"JSON Schema for Polly v8+ resilience pipeline configuration used in .NET applications with Microsoft.Extensions.Resilience.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResiliencePipelines\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/PipelineConfiguration\"\n      },\n      \"description\": \"Named resilience pipeline configurations.\"\n    }\n  },\n  \"$defs\": {\n    \"PipelineConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Retry\": {\n          \"$ref\": \"#/$defs/RetryStrategyOptions\"\n        },\n        \"CircuitBreaker\": {\n          \"$ref\": \"#/$defs/CircuitBreakerStrategyOptions\"\n        },\n        \"Timeout\"\
  : {\n          \"$ref\": \"#/$defs/TimeoutStrategyOptions\"\n        },\n        \"RateLimiter\": {\n          \"$ref\": \"#/$defs/RateLimiterStrategyOptions\"\n        },\n        \"Hedging\": {\n          \"$ref\": \"#/$defs/HedgingStrategyOptions\"\n        },\n        \"Fallback\": {\n          \"$ref\": \"#/$defs/FallbackStrategyOptions\"\n        }\n      }\n    },\n    \"RetryStrategyOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"MaxRetryAttempts\": {\n          \"type\": \"integer\",\n          \"default\": 3,\n          \"description\": \"Maximum number of retry attempts.\"\n        },\n        \"Delay\": {\n          \"type\": \"string\",\n          \"default\": \"00:00:02\",\n          \"description\": \"Base delay between retries (TimeSpan format).\"\n        },\n        \"MaxDelay\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum delay cap (TimeSpan format).\"\n        },\n        \"BackoffType\": {\n          \"type\"\
  : \"string\",\n          \"enum\": [\"Constant\", \"Linear\", \"Exponential\"],\n          \"default\": \"Constant\",\n          \"description\": \"Type of backoff strategy.\"\n        },\n        \"UseJitter\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether to add jitter to retry delays.\"\n        }\n      }\n    },\n    \"CircuitBreakerStrategyOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"FailureRatio\": {\n          \"type\": \"number\",\n          \"default\": 0.1,\n          \"description\": \"Failure ratio threshold to trip the circuit.\"\n        },\n        \"MinimumThroughput\": {\n          \"type\": \"integer\",\n          \"default\": 100,\n          \"description\": \"Minimum number of actions in the sampling duration.\"\n        },\n        \"SamplingDuration\": {\n          \"type\": \"string\",\n          \"default\": \"00:00:30\",\n          \"description\": \"Duration of the sampling\
  \ window (TimeSpan format).\"\n        },\n        \"BreakDuration\": {\n          \"type\": \"string\",\n          \"default\": \"00:00:05\",\n          \"description\": \"Duration the circuit remains open (TimeSpan format).\"\n        }\n      }\n    },\n    \"TimeoutStrategyOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Timeout\": {\n          \"type\": \"string\",\n          \"default\": \"00:00:30\",\n          \"description\": \"Timeout duration (TimeSpan format).\"\n        }\n      }\n    },\n    \"RateLimiterStrategyOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"PermitLimit\": {\n          \"type\": \"integer\",\n          \"default\": 1000,\n          \"description\": \"Maximum number of permits.\"\n        },\n        \"QueueLimit\": {\n          \"type\": \"integer\",\n          \"default\": 0,\n          \"description\": \"Maximum number of queued permits.\"\n        },\n        \"Window\": {\n          \"type\"\
  : \"string\",\n          \"default\": \"00:01:00\",\n          \"description\": \"Time window for rate limiting (TimeSpan format).\"\n        }\n      }\n    },\n    \"HedgingStrategyOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"MaxHedgedAttempts\": {\n          \"type\": \"integer\",\n          \"default\": 1,\n          \"description\": \"Maximum number of hedged attempts.\"\n        },\n        \"Delay\": {\n          \"type\": \"string\",\n          \"default\": \"00:00:02\",\n          \"description\": \"Delay before launching a hedged attempt (TimeSpan format).\"\n        }\n      }\n    },\n    \"FallbackStrategyOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"FallbackAction\": {\n          \"type\": \"string\",\n          \"description\": \"Name or reference to the fallback action handler.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polly/refs/heads/main/json-schema/resilience-pipeline-configuration.json
tags:
- .NET
- C#
- Circuit Breaker
- Fault Tolerance
- Microservices
- Rate Limiter
- Resilience
- Retry
- Timeout
title: Polly Resilience Pipeline Configuration
---
