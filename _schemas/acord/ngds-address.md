---
description: Address schema from ACORD NGDS API
layout: schema
name: Address
properties_list:
- description: ''
  name: street1
  type: string
- description: ''
  name: street2
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: country
  type: string
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-address-schema.json
slug: ngds-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"street1\": {\n      \"type\": \"string\"\n    },\n    \"street2\": {\n      \"type\": \"string\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"default\": \"US\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-address-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: Address
---
