---
description: Represents a Cloud Map service used for service discovery.
layout: schema
name: Service
properties_list:
- description: The ID of the service.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the service.
  name: Arn
  type: string
- description: The name of the service.
  name: Name
  type: string
- description: The ID of the namespace.
  name: NamespaceId
  type: string
- description: The description of the service.
  name: Description
  type: string
- description: The number of instances that are currently associated with the service.
  name: InstanceCount
  type: integer
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-service-schema.json
slug: cloud-map-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"Represents a Cloud Map service used for service discovery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the service.\",\n      \"example\": \"svc-abc12345\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the service.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service.\",\n      \"example\": \"payment-service\"\n    },\n    \"NamespaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the namespace.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description\
  \ of the service.\"\n    },\n    \"InstanceCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of instances that are currently associated with the service.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-service-schema.json
tags:
- AWS
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: Service
---
