---
description: An object that represents the backends that a virtual node is expected to send outbound traffic to.
layout: schema
name: Backend
properties_list:
- description: ''
  name: virtualService
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-backend-schema.json
slug: amazon-app-mesh-backend
source_filename: amazon-app-mesh-backend-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Backend\",\n  \"description\": \"An object that represents the backends that a virtual node is expected to send outbound traffic to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualService\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-backend-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: Backend
---
