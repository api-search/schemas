---
description: An API product exposed through the Gloo developer portal, containing metadata, versioning, visibility settings, and associated usage plans.
layout: schema
name: Solo.io Gloo Portal API Product
properties_list:
- description: Unique identifier for the API product.
  name: id
  type: string
- description: Name of the API product.
  name: name
  type: string
- description: Description of the API product.
  name: description
  type: string
- description: Version of the API product.
  name: version
  type: string
- description: Contact information for the API product owner.
  name: contact
  type: string
- description: License information for the API product.
  name: license
  type: string
- description: Terms of service URL.
  name: termsOfService
  type: string
- description: List of usage plan IDs associated with this API product.
  name: usagePlans
  type: array
- description: Available versions of this API.
  name: apiVersions
  type: array
- description: Visibility setting of the API product.
  name: visibility
  type: string
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/api-product.json
slug: api-product
source_filename: api-product.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/api-product.json\",\n  \"title\": \"Solo.io Gloo Portal API Product\",\n  \"description\": \"An API product exposed through the Gloo developer portal, containing metadata, versioning, visibility settings, and associated usage plans.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API product.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API product.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API product.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the API product.\"\n    },\n    \"contact\": {\n      \"type\": \"string\",\n      \"description\": \"Contact information for the\
  \ API product owner.\"\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"description\": \"License information for the API product.\"\n    },\n    \"termsOfService\": {\n      \"type\": \"string\",\n      \"description\": \"Terms of service URL.\"\n    },\n    \"usagePlans\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of usage plan IDs associated with this API product.\"\n    },\n    \"apiVersions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"api-version.json\"\n      },\n      \"description\": \"Available versions of this API.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"Visibility setting of the API product.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/api-product.json
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
title: Solo.io Gloo Portal API Product
---
