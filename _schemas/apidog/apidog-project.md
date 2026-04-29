---
description: Represents an Apidog project, the top-level container for endpoints, schemas, and environments managed through the Apidog API.
layout: schema
name: Apidog Project
properties_list:
- description: The unique identifier of the Apidog project.
  name: projectId
  type: integer
- description: The human-readable name of the project.
  name: name
  type: string
- description: A brief description of what this project contains.
  name: description
  type: string
- description: Total number of API endpoints in the project.
  name: endpointCount
  type: integer
- description: Total number of data schemas in the project.
  name: schemaCount
  type: integer
- description: Total number of environments configured in the project.
  name: environmentCount
  type: integer
- description: The Apidog API version used when interacting with this project.
  name: apiVersion
  type: string
provider_name: Apidog
provider_slug: apidog
schema_file: json-schema/apidog-project-schema.json
slug: apidog-project
source_filename: apidog-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/json-schema/apidog-project-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Apidog Project\",\n  \"description\": \"Represents an Apidog project, the top-level container for endpoints, schemas, and environments managed through the Apidog API.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"projectId\"\n  ],\n  \"properties\": {\n    \"projectId\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the Apidog project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the project.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of what this project contains.\"\n    },\n    \"endpointCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of API endpoints in the project.\"\
  ,\n      \"minimum\": 0\n    },\n    \"schemaCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of data schemas in the project.\",\n      \"minimum\": 0\n    },\n    \"environmentCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of environments configured in the project.\",\n      \"minimum\": 0\n    },\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The Apidog API version used when interacting with this project.\",\n      \"examples\": [\n        \"2024-03-28\"\n      ]\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/json-schema/apidog-project-schema.json
tags:
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- Mocking
- Platform
title: Apidog Project
---
