---
description: Response for creating a service.
layout: schema
name: CreateServiceResponse
properties_list:
- description: ''
  name: Service
  type: object
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-create-service-response-schema.json
slug: cloud-map-create-service-response
source_filename: cloud-map-create-service-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-create-service-response-schema.json\",\n  \"title\": \"CreateServiceResponse\",\n  \"description\": \"Response for creating a service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Service\": {\n      \"$ref\": \"#/components/schemas/Service\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-create-service-response-schema.json
tags:
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: CreateServiceResponse
---
