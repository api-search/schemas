---
description: An individual factor that contributed to the premium calculation
layout: schema
name: RatingFactor
properties_list:
- description: Name of the rating factor
  name: name
  type: string
- description: Value or level of the rating factor
  name: value
  type: string
- description: Human-readable description of the factor impact
  name: description
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-rating-factor-schema.json
slug: api-connect-rating-factor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-rating-factor-schema.json\",\n  \"title\": \"RatingFactor\",\n  \"description\": \"An individual factor that contributed to the premium calculation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the rating factor\",\n      \"example\": \"location_risk\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Value or level of the rating factor\",\n      \"example\": \"medium\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the factor impact\",\n      \"example\": \"Medium flood and bushfire risk area\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-rating-factor-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: RatingFactor
---
