---
description: Links schema from Adyen API
layout: schema
name: Links
properties_list:
- description: Link to the resource itself.
  name: self
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-links-schema.json
slug: management-links
source_filename: management-links-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-links-schema.json\",\n  \"title\": \"Links\",\n  \"description\": \"Links schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"self\": {\n      \"description\": \"Link to the resource itself.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    }\n  },\n  \"required\": [\n    \"self\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-links-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Links
---
