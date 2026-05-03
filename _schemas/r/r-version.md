---
description: Schema for an R release version record as returned by the METACRAN R Versions API
layout: schema
name: R Version
properties_list:
- description: R version number using major.minor.patch format
  name: version
  type: string
- description: Release date of this R version
  name: date
  type: string
- description: Release nickname assigned to this R version
  name: nickname
  type: string
provider_name: R
provider_slug: r
schema_file: json-schema/r-version-schema.json
slug: r-version
source_filename: r-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/json-schema/r-version-schema.json\",\n  \"title\": \"R Version\",\n  \"description\": \"Schema for an R release version record as returned by the METACRAN R Versions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"R version number using major.minor.patch format\",\n      \"example\": \"4.4.2\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Release date of this R version\",\n      \"example\": \"2024-10-31\"\n    },\n    \"nickname\": {\n      \"type\": \"string\",\n      \"description\": \"Release nickname assigned to this R version\",\n      \"example\": \"Pile of Leaves\"\n    }\n  },\n  \"required\": [\"version\", \"date\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/json-schema/r-version-schema.json
tags:
- R
- Statistics
- Data Science
- Open Source
- Programming Language
title: R Version
---
