---
description: ''
layout: schema
name: Feature
properties_list:
- description: Feature symbolic name
  name: name
  type: string
- description: Human-readable feature name
  name: displayName
  type: string
- description: Feature version
  name: version
  type: string
- description: Feature description
  name: description
  type: string
- description: Whether the feature is currently enabled
  name: enabled
  type: boolean
- description: List of dependent feature names
  name: dependencies
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-admin-rest-feature-schema.json
slug: websphere-liberty-admin-rest-feature
source_filename: websphere-liberty-admin-rest-feature-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Feature\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Feature symbolic name\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable feature name\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Feature version\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Feature description\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the feature is currently enabled\"\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"List of dependent feature names\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-admin-rest-feature-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Feature
---
