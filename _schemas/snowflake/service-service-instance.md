---
description: ''
layout: schema
name: ServiceInstance
properties_list:
- description: The current status of the service.
  name: service_status
  type: string
- description: ID of the service instance (this is the index of the service instance starting from 0).
  name: instance_id
  type: string
- description: The current status of the service instance.
  name: status
  type: string
- description: The unique and immutable identifier that represents the service specification content.
  name: spec_digest
  type: string
- description: The time when Snowflake started creating the service instance.
  name: creation_time
  type: string
- description: The time when Snowflake acknowledged the service instance is running on a node.
  name: start_time
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-service-instance-schema.json
slug: service-service-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceInstance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service_status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the service.\"\n    },\n    \"instance_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the service instance (this is the index of the service instance starting from 0).\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the service instance.\"\n    },\n    \"spec_digest\": {\n      \"type\": \"string\",\n      \"description\": \"The unique and immutable identifier that represents the service specification content.\"\n    },\n    \"creation_time\": {\n      \"type\": \"string\",\n      \"description\": \"The time when Snowflake started creating the service instance.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The time when Snowflake acknowledged the service instance is running on a node.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-service-instance-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ServiceInstance
---
