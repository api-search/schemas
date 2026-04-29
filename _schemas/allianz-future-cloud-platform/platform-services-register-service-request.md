---
description: Request body for registering a new service
layout: schema
name: RegisterServiceRequest
properties_list:
- description: Kebab-case service name
  name: name
  type: string
- description: Target Kubernetes namespace
  name: namespace
  type: string
- description: Primary programming language
  name: language
  type: string
- description: Git repository URL for the service
  name: repository_url
  type: string
- description: ''
  name: resource_requirements
  type: object
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-register-service-request-schema.json
slug: platform-services-register-service-request
source_filename: platform-services-register-service-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-register-service-request-schema.json\",\n  \"title\": \"RegisterServiceRequest\",\n  \"description\": \"Request body for registering a new service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Kebab-case service name\",\n      \"example\": \"claims-service\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Target Kubernetes namespace\",\n      \"example\": \"insurance-claims\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Primary programming language\",\n      \"enum\": [\n        \"kotlin\",\n        \"java\",\n        \"nodejs\",\n        \"python\"\n      ],\n      \"example\": \"kotlin\"\n    },\n    \"repository_url\":\
  \ {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Git repository URL for the service\",\n      \"example\": \"https://github.com/allianz/claims-service\"\n    },\n    \"resource_requirements\": {\n      \"$ref\": \"#/components/schemas/ResourceRequirements\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"namespace\",\n    \"language\",\n    \"repository_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-register-service-request-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: RegisterServiceRequest
---
