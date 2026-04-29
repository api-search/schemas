---
description: Location schema from Backstage catalog API
layout: schema
name: Location
properties_list:
- description: The unique identifier of the location.
  name: id
  type: string
- description: The type of the location (e.g., url, file).
  name: type
  type: string
- description: The target URL or path of the location.
  name: target
  type: string
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/catalog-location-schema.json
slug: catalog-location
source_filename: catalog-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/catalog-location-schema.json\",\n  \"title\": \"Location\",\n  \"description\": \"Location schema from Backstage catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the location.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the location (e.g., url, file).\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"The target URL or path of the location.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/catalog-location-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: Location
---
