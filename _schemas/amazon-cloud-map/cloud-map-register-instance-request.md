---
description: Request body for registering an instance.
layout: schema
name: RegisterInstanceRequest
properties_list:
- description: An identifier that you want to associate with the instance.
  name: InstanceId
  type: string
- description: A unique string that identifies the request and allows failed RegisterInstance requests to be retried.
  name: CreatorRequestId
  type: string
- description: A string map that contains the following information, including custom attributes.
  name: Attributes
  type: object
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-register-instance-request-schema.json
slug: cloud-map-register-instance-request
source_filename: cloud-map-register-instance-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-register-instance-request-schema.json\",\n  \"title\": \"RegisterInstanceRequest\",\n  \"description\": \"Request body for registering an instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"An identifier that you want to associate with the instance.\",\n      \"example\": \"i-1234567890abcdef0\"\n    },\n    \"CreatorRequestId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique string that identifies the request and allows failed RegisterInstance requests to be retried.\"\n    },\n    \"Attributes\": {\n      \"type\": \"object\",\n      \"description\": \"A string map that contains the following information, including custom attributes.\"\n    }\n  },\n  \"required\": [\n    \"InstanceId\"\
  ,\n    \"Attributes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-register-instance-request-schema.json
tags:
- AWS
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: RegisterInstanceRequest
---
