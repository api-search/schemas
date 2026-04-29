---
description: ''
layout: schema
name: deleted-item
properties_list:
- description: ''
  name: id
  type: object
- description: Date of deletion of the data in the platform and deletion of the metadata item if no other production status is defined.
  name: deletedDate
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-deleted-item-schema.json
slug: oneatlas-deleted-item
source_filename: oneatlas-deleted-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-deleted-item-schema.json\",\n  \"title\": \"deleted-item\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    },\n    \"deletedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date of deletion of the data in the platform and deletion of the metadata item if no other production status is defined.\\n\",\n      \"example\": \"2017-08-29T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-deleted-item-schema.json
tags:
- Imagery
- Satellites
title: deleted-item
---
