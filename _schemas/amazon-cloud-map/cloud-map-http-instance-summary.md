---
description: Represents a summary of a discovered service instance.
layout: schema
name: HttpInstanceSummary
properties_list:
- description: The ID of an instance.
  name: InstanceId
  type: string
- description: The HttpName name of the namespace.
  name: NamespaceName
  type: string
- description: The name of the service.
  name: ServiceName
  type: string
- description: If you configured health checking in the service, the current health status of the service's instances.
  name: HealthStatus
  type: string
- description: Custom attributes associated with the instance.
  name: Attributes
  type: object
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-http-instance-summary-schema.json
slug: cloud-map-http-instance-summary
source_filename: cloud-map-http-instance-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-http-instance-summary-schema.json\",\n  \"title\": \"HttpInstanceSummary\",\n  \"description\": \"Represents a summary of a discovered service instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of an instance.\",\n      \"example\": \"i-1234567890abcdef0\"\n    },\n    \"NamespaceName\": {\n      \"type\": \"string\",\n      \"description\": \"The HttpName name of the namespace.\",\n      \"example\": \"production.internal\"\n    },\n    \"ServiceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service.\",\n      \"example\": \"payment-service\"\n    },\n    \"HealthStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HEALTHY\",\n        \"UNHEALTHY\"\
  ,\n        \"UNKNOWN\"\n      ],\n      \"description\": \"If you configured health checking in the service, the current health status of the service's instances.\"\n    },\n    \"Attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Custom attributes associated with the instance.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-http-instance-summary-schema.json
tags:
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: HttpInstanceSummary
---
