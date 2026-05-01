---
description: Request body for discovering instances.
layout: schema
name: DiscoverInstancesRequest
properties_list:
- description: The HttpName name of the namespace.
  name: NamespaceName
  type: string
- description: The name of the service that you specified when you registered the instance.
  name: ServiceName
  type: string
- description: The maximum number of instances that you want Cloud Map to return.
  name: MaxResults
  type: integer
- description: The health status of the instances that you want to discover.
  name: HealthStatus
  type: string
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-discover-instances-request-schema.json
slug: cloud-map-discover-instances-request
source_filename: cloud-map-discover-instances-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-discover-instances-request-schema.json\",\n  \"title\": \"DiscoverInstancesRequest\",\n  \"description\": \"Request body for discovering instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NamespaceName\": {\n      \"type\": \"string\",\n      \"description\": \"The HttpName name of the namespace.\",\n      \"example\": \"production.internal\"\n    },\n    \"ServiceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service that you specified when you registered the instance.\",\n      \"example\": \"payment-service\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of instances that you want Cloud Map to return.\"\n    },\n    \"HealthStatus\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\n        \"HEALTHY\",\n        \"UNHEALTHY\",\n        \"ALL\",\n        \"HEALTHY_OR_ELSE_ALL\"\n      ],\n      \"description\": \"The health status of the instances that you want to discover.\"\n    }\n  },\n  \"required\": [\n    \"NamespaceName\",\n    \"ServiceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-discover-instances-request-schema.json
tags:
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: DiscoverInstancesRequest
---
