---
description: Lists the required security schemes to execute an operation. Each name must correspond to a security scheme declared in the Security Schemes under the Components Object.
layout: schema
name: OpenAPI Security Requirement Object
properties_list: []
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-security-requirement.json
slug: openapi-security-requirement
source_filename: openapi-security-requirement.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-security-requirement.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Security Requirement Object\",\n  \"description\": \"Lists the required security schemes to execute an operation. Each name must correspond to a security scheme declared in the Security Schemes under the Components Object.\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"array\",\n    \"items\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-security-requirement.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Security Requirement Object
---
