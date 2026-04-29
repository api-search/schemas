---
description: ''
layout: schema
name: ServiceEndpoint
properties_list:
- description: User-friendly endpoint name that represents the corresponding port.
  name: name
  type: string
- description: The network port the service is listening on. NULL, when portRange is specified.
  name: port
  type: integer
- description: The network port range the service is listening on. NULL, when port is specified.
  name: portRange
  type: string
- description: Supported network protocol (TCP, HTTP, or HTTPS).
  name: protocol
  type: string
- description: True, if the endpoint is public, accessible from internet.
  name: is_public
  type: boolean
- description: Endpoint URL accessible from the internet.
  name: ingress_url
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-service-endpoint-schema.json
slug: service-service-endpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceEndpoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User-friendly endpoint name that represents the corresponding port.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The network port the service is listening on. NULL, when portRange is specified.\"\n    },\n    \"portRange\": {\n      \"type\": \"string\",\n      \"description\": \"The network port range the service is listening on. NULL, when port is specified.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Supported network protocol (TCP, HTTP, or HTTPS).\"\n    },\n    \"is_public\": {\n      \"type\": \"boolean\",\n      \"description\": \"True, if the endpoint is public, accessible from internet.\"\n    },\n    \"ingress_url\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Endpoint URL accessible from the internet.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-service-endpoint-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ServiceEndpoint
---
