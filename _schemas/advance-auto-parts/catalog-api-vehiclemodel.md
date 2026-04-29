---
description: A vehicle model.
layout: schema
name: VehicleModel
properties_list:
- description: Model identifier.
  name: id
  type: string
- description: Model display name.
  name: name
  type: string
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-vehiclemodel-schema.json
slug: catalog-api-vehiclemodel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VehicleModel\",\n  \"description\": \"A vehicle model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Model identifier.\",\n      \"example\": \"F150\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Model display name.\",\n      \"example\": \"F-150\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-vehiclemodel-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: VehicleModel
---
