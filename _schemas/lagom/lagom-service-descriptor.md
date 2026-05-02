---
description: JSON Schema representing the structure of a Lagom service descriptor, defining service calls, topics, and ACLs.
layout: schema
name: Lagom Service Descriptor
properties_list:
- description: The name of the service.
  name: name
  type: string
- description: List of service call definitions.
  name: calls
  type: array
- description: List of topic definitions for event publishing.
  name: topics
  type: array
- description: Access control list entries.
  name: acls
  type: array
provider_name: Lagom
provider_slug: lagom
schema_file: json-schema/lagom-service-descriptor.json
slug: lagom-service-descriptor
source_filename: lagom-service-descriptor.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/lagom/json-schema/lagom-service-descriptor.json\",\n  \"title\": \"Lagom Service Descriptor\",\n  \"description\": \"JSON Schema representing the structure of a Lagom service descriptor, defining service calls, topics, and ACLs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service.\"\n    },\n    \"calls\": {\n      \"type\": \"array\",\n      \"description\": \"List of service call definitions.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the service call.\"\n          },\n          \"method\": {\n            \"type\": \"string\",\n            \"description\": \"HTTP method for the call.\",\n            \"enum\": [\"GET\", \"POST\", \"PUT\"\
  , \"DELETE\", \"PATCH\", \"HEAD\", \"OPTIONS\"]\n          },\n          \"path\": {\n            \"type\": \"string\",\n            \"description\": \"URL path pattern for the call (e.g., /api/items/:id).\"\n          },\n          \"circuitBreaker\": {\n            \"type\": \"object\",\n            \"description\": \"Circuit breaker configuration for this call.\",\n            \"properties\": {\n              \"enabled\": {\n                \"type\": \"boolean\",\n                \"default\": true\n              },\n              \"maxFailures\": {\n                \"type\": \"integer\",\n                \"default\": 10\n              },\n              \"callTimeout\": {\n                \"type\": \"string\",\n                \"description\": \"Duration string (e.g., 10s).\",\n                \"default\": \"10s\"\n              },\n              \"resetTimeout\": {\n                \"type\": \"string\",\n                \"description\": \"Duration string (e.g., 15s).\",\n          \
  \      \"default\": \"15s\"\n              }\n            },\n            \"additionalProperties\": true\n          },\n          \"autoAcl\": {\n            \"type\": \"boolean\",\n            \"description\": \"Automatically generate ACL for this call.\",\n            \"default\": true\n          }\n        },\n        \"required\": [\"name\", \"path\"],\n        \"additionalProperties\": true\n      }\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"description\": \"List of topic definitions for event publishing.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Topic name.\"\n          },\n          \"partitionKeyStrategy\": {\n            \"type\": \"string\",\n            \"description\": \"Fully qualified class name of the partition key strategy.\"\n          }\n        },\n        \"required\": [\"name\"],\n        \"additionalProperties\": true\n\
  \      }\n    },\n    \"acls\": {\n      \"type\": \"array\",\n      \"description\": \"Access control list entries.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"method\": {\n            \"type\": \"string\",\n            \"enum\": [\"GET\", \"POST\", \"PUT\", \"DELETE\", \"PATCH\", \"HEAD\", \"OPTIONS\"]\n          },\n          \"pathRegex\": {\n            \"type\": \"string\",\n            \"description\": \"Regex pattern for matching request paths.\"\n          }\n        },\n        \"additionalProperties\": true\n      }\n    }\n  },\n  \"required\": [\"name\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lagom/refs/heads/main/json-schema/lagom-service-descriptor.json
tags:
- Akka
- Event Sourcing
- Frameworks
- Java
- Microservices
- Reactive
- Scala
title: Lagom Service Descriptor
---
