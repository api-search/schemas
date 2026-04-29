---
description: Response object for Entity Matches.
layout: schema
name: EntityMatchesResponse
properties_list:
- description: Candidate list of `Entity Match` objects.
  name: data
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-private-markets-entity-matches-response-schema.json
slug: factset-private-markets-entity-matches-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EntityMatchesResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response object for Entity Matches.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Candidate list of `Entity Match` objects.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-private-markets-entity-matches-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: EntityMatchesResponse
---
