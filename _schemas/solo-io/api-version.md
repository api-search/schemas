---
description: A version of an API product, specifying the schema type used for its definition.
layout: schema
name: Solo.io Gloo Portal API Version
properties_list:
- description: Unique identifier for the API version.
  name: id
  type: string
- description: Version string.
  name: version
  type: string
- description: Type of schema for this API version.
  name: schemaType
  type: string
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/api-version.json
slug: api-version
source_filename: api-version.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/api-version.json\",\n  \"title\": \"Solo.io Gloo Portal API Version\",\n  \"description\": \"A version of an API product, specifying the schema type used for its definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API version.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version string.\"\n    },\n    \"schemaType\": {\n      \"type\": \"string\",\n      \"enum\": [\"openapi\", \"graphql\", \"grpc\"],\n      \"description\": \"Type of schema for this API version.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/api-version.json
tags:
- AI Gateway
- Analytics
- Automation
- Gateways
- Management
- Monetization
- Observability
- Platform
- Resiliency
- Security
- Service Mesh
- Traffic Control
title: Solo.io Gloo Portal API Version
---
