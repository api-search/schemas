---
description: Request body for creating a service.
layout: schema
name: CreateServiceRequest
properties_list:
- description: The name that you want to assign to the service.
  name: Name
  type: string
- description: The ID of the namespace that you want to use to create the service.
  name: NamespaceId
  type: string
- description: A description for the service.
  name: Description
  type: string
- description: A complex type that contains information about the Amazon Route 53 records that you want AWS Cloud Map to create when you register an instance.
  name: DnsConfig
  type: object
- description: A unique string that identifies the request and allows failed CreateService requests to be retried.
  name: CreatorRequestId
  type: string
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-create-service-request-schema.json
slug: cloud-map-create-service-request
source_filename: cloud-map-create-service-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-create-service-request-schema.json\",\n  \"title\": \"CreateServiceRequest\",\n  \"description\": \"Request body for creating a service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name that you want to assign to the service.\",\n      \"example\": \"payment-service\"\n    },\n    \"NamespaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the namespace that you want to use to create the service.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description for the service.\"\n    },\n    \"DnsConfig\": {\n      \"type\": \"object\",\n      \"description\": \"A complex type that contains information about the Amazon Route 53 records that you want AWS\
  \ Cloud Map to create when you register an instance.\"\n    },\n    \"CreatorRequestId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique string that identifies the request and allows failed CreateService requests to be retried.\"\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-create-service-request-schema.json
tags:
- AWS
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: CreateServiceRequest
---
