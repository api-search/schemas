---
description: Represents an instance registered with a Cloud Map service.
layout: schema
name: Instance
properties_list:
- description: An identifier that you want to associate with the instance.
  name: Id
  type: string
- description: Custom attributes associated with the instance.
  name: Attributes
  type: object
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-instance-schema.json
slug: cloud-map-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-instance-schema.json\",\n  \"title\": \"Instance\",\n  \"description\": \"Represents an instance registered with a Cloud Map service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"An identifier that you want to associate with the instance.\",\n      \"example\": \"i-1234567890abcdef0\"\n    },\n    \"Attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Custom attributes associated with the instance.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-instance-schema.json
tags:
- AWS
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: Instance
---
