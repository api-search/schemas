---
description: An organizational department from a connected HRIS system.
layout: schema
name: Department
properties_list:
- description: Department ID.
  name: id
  type: string
- description: Department name.
  name: name
  type: string
- description: Parent department ID for nested structures.
  name: parent_id
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-department-schema.json
slug: bindbee-department
source_filename: bindbee-department-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Department\",\n  \"type\": \"object\",\n  \"description\": \"An organizational department from a connected HRIS system.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Department ID.\",\n      \"example\": \"dept-abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Department name.\",\n      \"example\": \"Engineering\"\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Parent department ID for nested structures.\",\n      \"example\": null\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-department-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: Department
---
