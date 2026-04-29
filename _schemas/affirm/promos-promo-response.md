---
description: Response containing promotional messaging content and financing offer details for the requested purchase amount.
layout: schema
name: PromoResponse
properties_list:
- description: ''
  name: promo
  type: object
- description: ''
  name: offer
  type: object
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/promos-promo-response-schema.json
slug: promos-promo-response
source_filename: promos-promo-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-promo-response-schema.json\",\n  \"title\": \"PromoResponse\",\n  \"description\": \"Response containing promotional messaging content and financing offer details for the requested purchase amount.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"promo\": {\n      \"$ref\": \"#/components/schemas/PromoContent\"\n    },\n    \"offer\": {\n      \"$ref\": \"#/components/schemas/OfferContent\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-promo-response-schema.json
tags: []
title: PromoResponse
---
