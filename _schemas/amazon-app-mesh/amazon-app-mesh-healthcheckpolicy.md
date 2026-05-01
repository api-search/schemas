---
description: An object that represents the health check policy for a virtual node's listener.
layout: schema
name: HealthCheckPolicy
properties_list:
- description: ''
  name: healthyThreshold
  type: object
- description: ''
  name: intervalMillis
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: port
  type: object
- description: ''
  name: protocol
  type: object
- description: ''
  name: timeoutMillis
  type: object
- description: ''
  name: unhealthyThreshold
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-healthcheckpolicy-schema.json
slug: amazon-app-mesh-healthcheckpolicy
source_filename: amazon-app-mesh-healthcheckpolicy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HealthCheckPolicy\",\n  \"description\": \"An object that represents the health check policy for a virtual node's listener.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"healthyThreshold\": {},\n    \"intervalMillis\": {},\n    \"path\": {},\n    \"port\": {},\n    \"protocol\": {},\n    \"timeoutMillis\": {},\n    \"unhealthyThreshold\": {}\n  },\n  \"required\": [\n    \"healthyThreshold\",\n    \"intervalMillis\",\n    \"protocol\",\n    \"timeoutMillis\",\n    \"unhealthyThreshold\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-healthcheckpolicy-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: HealthCheckPolicy
---
