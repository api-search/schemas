---
description: Schema for a request in progress response returned by the server.
layout: schema
name: SuccessAcceptedResponse
properties_list:
- description: Message code returned by the server.
  name: code
  type: string
- description: Message returned by the server
  name: message
  type: string
- description: Opaque result ID used for checking for request completion through one or more subsequent completion check operations.
  name: resultHandler
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-success-accepted-response-schema.json
slug: common-success-accepted-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessAcceptedResponse\",\n  \"type\": \"object\",\n  \"description\": \"Schema for a request in progress response returned by the server.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Message code returned by the server.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Message returned by the server\"\n    },\n    \"resultHandler\": {\n      \"type\": \"string\",\n      \"description\": \"Opaque result ID used for checking for request completion through one or more subsequent completion check operations.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-success-accepted-response-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: SuccessAcceptedResponse
---
