---
description: A vehicle manufacturer.
layout: schema
name: Make
properties_list:
- description: Make identifier.
  name: id
  type: string
- description: Make display name.
  name: name
  type: string
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-make-schema.json
slug: catalog-api-make
source_filename: catalog-api-make-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Make\",\n  \"description\": \"A vehicle manufacturer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Make identifier.\",\n      \"example\": \"FORD\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Make display name.\",\n      \"example\": \"Ford\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-make-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: Make
---
