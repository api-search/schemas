---
description: Address schema from ARGUS Enterprise API
layout: schema
name: Address
properties_list:
- description: Street address
  name: street
  type: string
- description: City
  name: city
  type: string
- description: State or province
  name: state
  type: string
- description: Postal or ZIP code
  name: postalCode
  type: string
- description: Country code (ISO 3166-1 alpha-2)
  name: country
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-address-schema.json
slug: argus-enterprise-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"street\": {\n      \"type\": \"string\",\n      \"description\": \"Street address\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code (ISO 3166-1 alpha-2)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-address-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Address
---
