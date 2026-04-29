---
description: Information about invalid request parameter.
layout: schema
name: InvalidParam
properties_list:
- description: Parameter name.
  name: name
  type: string
- description: The issue with the parameter.
  name: reason
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-invalid-param-schema.json
slug: rest-api-invalid-param
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-invalid-param-schema.json\",\n  \"title\": \"InvalidParam\",\n  \"description\": \"Information about invalid request parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter name.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"The issue with the parameter.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-invalid-param-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: InvalidParam
---
