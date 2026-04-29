---
description: Specifies service specification.
layout: schema
name: ServiceSpec
properties_list:
- description: Type of the service specification, can be `from_file` or `from_inline`.
  name: spec_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-service-spec-schema.json
slug: service-service-spec
source_filename: service-service-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specifies service specification.\",\n  \"properties\": {\n    \"spec_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the service specification, can be `from_file` or `from_inline`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-service-spec-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ServiceSpec
---
