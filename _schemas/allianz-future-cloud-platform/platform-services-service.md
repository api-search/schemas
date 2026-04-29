---
description: A microservice registered on the Allianz Future Cloud Platform
layout: schema
name: Service
properties_list:
- description: Unique identifier for the service
  name: service_id
  type: string
- description: Kebab-case service name
  name: name
  type: string
- description: Kubernetes namespace the service belongs to
  name: namespace
  type: string
- description: Current operational status
  name: status
  type: string
- description: Number of running pod replicas
  name: replicas
  type: integer
- description: Currently deployed version
  name: version
  type: string
- description: Primary programming language
  name: language
  type: string
- description: Git repository URL
  name: repository_url
  type: string
- description: Timestamp when the service was registered
  name: created_at
  type: string
- description: Timestamp when the service was last updated
  name: modified_at
  type: string
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-service-schema.json
slug: platform-services-service
source_filename: platform-services-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"A microservice registered on the Allianz Future Cloud Platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the service\",\n      \"example\": \"svc-500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Kebab-case service name\",\n      \"example\": \"policy-service\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes namespace the service belongs to\",\n      \"example\": \"insurance-policy\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status\",\n      \"enum\"\
  : [\n        \"running\",\n        \"pending\",\n        \"failed\",\n        \"stopped\"\n      ],\n      \"example\": \"running\"\n    },\n    \"replicas\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of running pod replicas\",\n      \"example\": 3\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Currently deployed version\",\n      \"example\": \"2.5.1\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Primary programming language\",\n      \"enum\": [\n        \"kotlin\",\n        \"java\",\n        \"nodejs\",\n        \"python\"\n      ],\n      \"example\": \"kotlin\"\n    },\n    \"repository_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Git repository URL\",\n      \"example\": \"https://github.com/allianz/policy-service\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"\
  Timestamp when the service was registered\",\n      \"example\": \"2026-01-01T00:00:00Z\"\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the service was last updated\",\n      \"example\": \"2026-04-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-service-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: Service
---
