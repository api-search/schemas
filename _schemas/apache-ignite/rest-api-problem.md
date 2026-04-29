---
description: Extended description of the problem with the request.
layout: schema
name: Problem
properties_list:
- description: Short summary of the issue.
  name: title
  type: string
- description: Returned HTTP status code.
  name: status
  type: integer
- description: Ignite 3 error code.
  name: code
  type: string
- description: URI to documentation regarding the issue.
  name: type
  type: string
- description: Extended explanation of the issue.
  name: detail
  type: string
- description: Name of the node the issue happened on.
  name: node
  type: string
- description: Unique issue identifier. This identifier can be used to find logs related to the issue.
  name: traceId
  type: string
- description: A list of parameters that did not pass validation and the reason for it.
  name: invalidParams
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-problem-schema.json
slug: rest-api-problem
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-problem-schema.json\",\n  \"title\": \"Problem\",\n  \"description\": \"Extended description of the problem with the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short summary of the issue.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"Returned HTTP status code.\",\n      \"format\": \"int32\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Ignite 3 error code.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"URI to documentation regarding the issue.\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Extended explanation of the issue.\"\n    },\n    \"node\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Name of the node the issue happened on.\"\n    },\n    \"traceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique issue identifier. This identifier can be used to find logs related to the issue.\",\n      \"format\": \"uuid\"\n    },\n    \"invalidParams\": {\n      \"type\": \"array\",\n      \"description\": \"A list of parameters that did not pass validation and the reason for it.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InvalidParam\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-problem-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: Problem
---
