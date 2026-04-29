---
description: ''
layout: schema
name: RatingConfigDto
properties_list:
- description: ''
  name: ratingsVisibleToAuthor
  type: boolean
- description: ''
  name: ratingsVisibleToViewers
  type: boolean
- description: ''
  name: ratingsVisibleToAll
  type: boolean
- description: ''
  name: viewerIds
  type: array
- description: ''
  name: optionValues
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-configuration-rating-config-dto-schema.json
slug: factset-irn-configuration-rating-config-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RatingConfigDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ratingsVisibleToAuthor\": {\n      \"type\": \"boolean\"\n    },\n    \"ratingsVisibleToViewers\": {\n      \"type\": \"boolean\"\n    },\n    \"ratingsVisibleToAll\": {\n      \"type\": \"boolean\"\n    },\n    \"viewerIds\": {\n      \"type\": \"array\"\n    },\n    \"optionValues\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-configuration-rating-config-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: RatingConfigDto
---
