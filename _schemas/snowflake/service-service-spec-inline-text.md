---
description: Specifies service specification with inline text.
layout: schema
name: ServiceSpecInlineText
properties_list:
- description: Specifies service specification. You can use a pair of dollar signs ($$) to delimit the beginning and ending of the specification string.
  name: spec_text
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-service-spec-inline-text-schema.json
slug: service-service-spec-inline-text
source_filename: service-service-spec-inline-text-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceSpecInlineText\",\n  \"type\": \"object\",\n  \"description\": \"Specifies service specification with inline text.\",\n  \"properties\": {\n    \"spec_text\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies service specification. You can use a pair of dollar signs ($$) to delimit the beginning and ending of the specification string.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-service-spec-inline-text-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ServiceSpecInlineText
---
