---
description: ''
layout: schema
name: ServiceContainer
properties_list:
- description: The current status of the service.
  name: service_status
  type: string
- description: ID of the service instance (this is the index of the service instance starting from 0).
  name: instance_id
  type: string
- description: The current status of the service instance.
  name: instance_status
  type: string
- description: Name of the container.
  name: container_name
  type: string
- description: Service container status.
  name: status
  type: string
- description: Additional clarification about status.
  name: message
  type: string
- description: Image name used to create the service container.
  name: image_name
  type: string
- description: The unique and immutable identifier representing the image content.
  name: image_digest
  type: string
- description: Number of times Snowflake restarted the service.
  name: restart_count
  type: integer
- description: Date and time when the container started.
  name: start_time
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-service-container-schema.json
slug: service-service-container
source_filename: service-service-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceContainer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service_status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the service.\"\n    },\n    \"instance_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the service instance (this is the index of the service instance starting from 0).\"\n    },\n    \"instance_status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the service instance.\"\n    },\n    \"container_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the container.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Service container status.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Additional clarification about status.\"\n    },\n    \"image_name\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Image name used to create the service container.\"\n    },\n    \"image_digest\": {\n      \"type\": \"string\",\n      \"description\": \"The unique and immutable identifier representing the image content.\"\n    },\n    \"restart_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times Snowflake restarted the service.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the container started.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-service-container-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ServiceContainer
---
