---
description: An application in the Choreo developer portal, representing a logical consumer of APIs such as a mobile app, web app, or device.
layout: schema
name: Choreo Application
properties_list:
- description: Unique identifier for the application.
  name: id
  type: string
- description: Name of the application.
  name: name
  type: string
- description: Description of the application.
  name: description
  type: string
- description: Throttling policy applied to the application.
  name: throttlingPolicy
  type: string
- description: Current status of the application.
  name: status
  type: string
- description: Timestamp when the application was created.
  name: createdAt
  type: string
provider_name: Choreo
provider_slug: choreo
schema_file: json-schema/choreo-application.json
slug: choreo-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-application.json\",\n  \"title\": \"Choreo Application\",\n  \"description\": \"An application in the Choreo developer portal, representing a logical consumer of APIs such as a mobile app, web app, or device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the application.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the application.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the application.\"\n    },\n    \"throttlingPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Throttling policy applied to the application.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"APPROVED\"\
  , \"CREATED\", \"REJECTED\"],\n      \"description\": \"Current status of the application.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the application was created.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"throttlingPolicy\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/json-schema/choreo-application.json
tags:
- AI Apps
- API Management
- CI/CD
- Cloud Native
- DevOps
- Developer Portal
- FinOps
- IDE
- Internal Developer Platform
- Kubernetes
- Lifecycle
- Observability
- Orchestration
- Platform Engineering
- Pro-Code API Composition
- Unified
- WSO2
- Workflows
title: Choreo Application
---
