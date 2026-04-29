---
description: Schema for a service definition registered with the Consul agent or catalog.
layout: schema
name: Consul Service Definition
properties_list:
- description: ''
  name: ID
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: Tags
  type: array
- description: ''
  name: Address
  type: string
- description: ''
  name: TaggedAddresses
  type: object
- description: ''
  name: Meta
  type: object
- description: ''
  name: Port
  type: integer
- description: ''
  name: Kind
  type: string
- description: ''
  name: Proxy
  type: object
- description: ''
  name: Connect
  type: object
- description: ''
  name: Weights
  type: object
- description: ''
  name: Check
  type: object
- description: ''
  name: Checks
  type: array
- description: ''
  name: EnableTagOverride
  type: boolean
- description: ''
  name: Namespace
  type: string
- description: ''
  name: Partition
  type: string
provider_name: HashiCorp Consul
provider_slug: consul
schema_file: json-schema/consul-service-schema.json
slug: consul-service
source_filename: consul-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/json-schema/consul-service-schema.json\",\n  \"title\": \"Consul Service Definition\",\n  \"description\": \"Schema for a service definition registered with the Consul agent or catalog.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": { \"type\": \"string\" },\n    \"Name\": { \"type\": \"string\" },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"Address\": { \"type\": \"string\" },\n    \"TaggedAddresses\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Address\": { \"type\": \"string\" },\n          \"Port\": { \"type\": \"integer\" }\n        }\n      }\n    },\n    \"Meta\": {\n      \"type\": \"object\",\n      \"additionalProperties\": { \"type\": \"string\" }\n   \
  \ },\n    \"Port\": { \"type\": \"integer\", \"minimum\": 1, \"maximum\": 65535 },\n    \"Kind\": {\n      \"type\": \"string\",\n      \"enum\": [\"\", \"connect-proxy\", \"mesh-gateway\", \"ingress-gateway\", \"terminating-gateway\"]\n    },\n    \"Proxy\": { \"type\": \"object\" },\n    \"Connect\": { \"type\": \"object\" },\n    \"Weights\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Passing\": { \"type\": \"integer\" },\n        \"Warning\": { \"type\": \"integer\" }\n      }\n    },\n    \"Check\": { \"$ref\": \"#/definitions/HealthCheck\" },\n    \"Checks\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/definitions/HealthCheck\" }\n    },\n    \"EnableTagOverride\": { \"type\": \"boolean\" },\n    \"Namespace\": { \"type\": \"string\" },\n    \"Partition\": { \"type\": \"string\" }\n  },\n  \"required\": [\"Name\"],\n  \"definitions\": {\n    \"HealthCheck\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"CheckID\": {\
  \ \"type\": \"string\" },\n        \"Name\": { \"type\": \"string\" },\n        \"Notes\": { \"type\": \"string\" },\n        \"Status\": {\n          \"type\": \"string\",\n          \"enum\": [\"passing\", \"warning\", \"critical\", \"maintenance\"]\n        },\n        \"HTTP\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"TCP\": { \"type\": \"string\" },\n        \"gRPC\": { \"type\": \"string\" },\n        \"Method\": { \"type\": \"string\" },\n        \"Header\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          }\n        },\n        \"TLSSkipVerify\": { \"type\": \"boolean\" },\n        \"Interval\": { \"type\": \"string\" },\n        \"Timeout\": { \"type\": \"string\" },\n        \"DeregisterCriticalServiceAfter\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/json-schema/consul-service-schema.json
tags:
- ACL
- Configuration
- Health Checking
- Key/Value Store
- Multi-Datacenter
- Open Source
- Service Discovery
- Service Mesh
title: Consul Service Definition
---
