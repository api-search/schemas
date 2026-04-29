---
description: Response for registering an instance.
layout: schema
name: RegisterInstanceResponse
properties_list:
- description: A value that you can use to determine whether the request completed successfully.
  name: OperationId
  type: string
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-register-instance-response-schema.json
slug: cloud-map-register-instance-response
source_filename: cloud-map-register-instance-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-register-instance-response-schema.json\",\n  \"title\": \"RegisterInstanceResponse\",\n  \"description\": \"Response for registering an instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OperationId\": {\n      \"type\": \"string\",\n      \"description\": \"A value that you can use to determine whether the request completed successfully.\",\n      \"example\": \"op-abc12345\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-register-instance-response-schema.json
tags:
- AWS
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: RegisterInstanceResponse
---
