---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: Error message returned by the server
  name: message
  type: string
- description: Error code.
  name: code
  type: string
- description: Error code, same as `code` above. This property has been deprecated and will be removed in a future release, but is temporarily supported for for short-term backward compatibility.
  name: error_code
  type: string
- description: Unique request ID.
  name: request_id
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-error-response-schema.json
slug: common-error-response
source_filename: common-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message returned by the server\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code.\"\n    },\n    \"error_code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code, same as `code` above. This property has been deprecated and will be removed in a future release, but is temporarily supported for for short-term backward compatibility.\"\n    },\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique request ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-error-response-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ErrorResponse
---
