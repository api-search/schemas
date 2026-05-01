---
description: A service configured in a DreamFactory instance, representing a connectable resource such as a database, file storage, remote API, or scripting endpoint.
layout: schema
name: DreamFactory Service
properties_list:
- description: Unique identifier for the service.
  name: id
  type: integer
- description: Unique name for the service, used in API paths.
  name: name
  type: string
- description: Display label for the service.
  name: label
  type: string
- description: Description of the service.
  name: description
  type: string
- description: Service type name identifying the connector.
  name: type
  type: string
- description: Whether the service is active.
  name: is_active
  type: boolean
- description: Service configuration object. Schema varies by service type.
  name: config
  type: object
- description: Timestamp when the service was created.
  name: created_date
  type: string
- description: Timestamp when the service was last modified.
  name: last_modified_date
  type: string
provider_name: DreamFactory
provider_slug: dreamfactory
schema_file: json-schema/dreamfactory-service.json
slug: dreamfactory-service
source_filename: dreamfactory-service.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-service.json\",\n  \"title\": \"DreamFactory Service\",\n  \"description\": \"A service configured in a DreamFactory instance, representing a connectable resource such as a database, file storage, remote API, or scripting endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the service.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the service, used in API paths.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label for the service.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the service.\"\n    },\n    \"type\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Service type name identifying the connector.\"\n    },\n    \"is_active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the service is active.\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Service configuration object. Schema varies by service type.\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the service was created.\"\n    },\n    \"last_modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the service was last modified.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/json-schema/dreamfactory-service.json
tags:
- Automation
- Deployment
- Documentation
- Generation
- Security
title: DreamFactory Service
---
