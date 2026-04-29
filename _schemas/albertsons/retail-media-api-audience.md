---
description: An audience targeting segment based on shopper behavior.
layout: schema
name: Audience
properties_list:
- description: Unique identifier of the audience segment.
  name: audienceId
  type: string
- description: Display name of the audience segment.
  name: name
  type: string
- description: Description of the audience segment criteria.
  name: description
  type: string
- description: Approximate number of shoppers in the audience segment.
  name: size
  type: integer
- description: Product category associated with the audience.
  name: category
  type: string
provider_name: albertsons
provider_slug: albertsons
schema_file: json-schema/retail-media-api-audience-schema.json
slug: retail-media-api-audience
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-audience-schema.json\",\n  \"title\": \"Audience\",\n  \"description\": \"An audience targeting segment based on shopper behavior.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"audienceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the audience segment.\",\n      \"example\": \"aud-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the audience segment.\",\n      \"example\": \"Organic Food Buyers\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the audience segment criteria.\",\n      \"example\": \"Shoppers with high organic product purchase frequency\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate\
  \ number of shoppers in the audience segment.\",\n      \"example\": 2500000\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category associated with the audience.\",\n      \"example\": \"grocery\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-audience-schema.json
tags:
- Grocery
- Retail
- Retail Media
- Advertising
- Campaigns
- Analytics
- Consumer Goods
- Food
- Pharmacy
title: Audience
---
