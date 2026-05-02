---
description: An API Specification represents an OpenAPI document managed through the Jetic API Builder, which can be linked to an integration for generating REST API endpoints.
layout: schema
name: Jetic API Specification
properties_list:
- description: Unique specification identifier.
  name: id
  type: string
- description: Name of the API specification.
  name: name
  type: string
- description: Description of the API.
  name: description
  type: string
- description: API version string.
  name: version
  type: string
- description: OpenAPI specification version.
  name: openApiVersion
  type: string
- description: Number of paths defined in the specification.
  name: paths
  type: integer
- description: Associated integration identifier.
  name: integrationId
  type: string
- description: Timestamp when the specification was created.
  name: createdAt
  type: string
- description: Timestamp when the specification was last updated.
  name: updatedAt
  type: string
provider_name: Jetic
provider_slug: jetic
schema_file: json-schema/api-specification.json
slug: api-specification
source_filename: api-specification.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/jetic/blob/main/json-schema/api-specification.json\",\n  \"title\": \"Jetic API Specification\",\n  \"description\": \"An API Specification represents an OpenAPI document managed through the Jetic API Builder, which can be linked to an integration for generating REST API endpoints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique specification identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API specification.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"API version string.\"\n    },\n    \"openApiVersion\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"3.0\",\n \
  \       \"3.1\"\n      ],\n      \"description\": \"OpenAPI specification version.\"\n    },\n    \"paths\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of paths defined in the specification.\"\n    },\n    \"integrationId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated integration identifier.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the specification was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the specification was last updated.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/json-schema/api-specification.json
tags:
- Apache Camel
- Integrations
- iPaaS
- Pro-Code API Composition
title: Jetic API Specification
---
