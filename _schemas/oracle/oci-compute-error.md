---
description: Error response returned by the OCI API
layout: schema
name: Error
properties_list:
- description: A short error code that defines the error, meant for programmatic parsing
  name: code
  type: string
- description: A human-readable error string
  name: message
  type: string
- description: The HTTP status code
  name: status
  type: integer
- description: Unique Oracle-assigned identifier for the request
  name: opcRequestId
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-error-schema.json
slug: oci-compute-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Error response returned by the OCI API\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"A short error code that defines the error, meant for programmatic parsing\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error string\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code\"\n    },\n    \"opcRequestId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Oracle-assigned identifier for the request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-error-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: Error
---
