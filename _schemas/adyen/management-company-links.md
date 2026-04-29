---
description: CompanyLinks schema from Adyen API
layout: schema
name: CompanyLinks
properties_list:
- description: ''
  name: apiCredentials
  type: object
- description: Link to the resource itself.
  name: self
  type: object
- description: ''
  name: users
  type: object
- description: ''
  name: webhooks
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-company-links-schema.json
slug: management-company-links
source_filename: management-company-links-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-company-links-schema.json\",\n  \"title\": \"CompanyLinks\",\n  \"description\": \"CompanyLinks schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiCredentials\": {\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"self\": {\n      \"description\": \"Link to the resource itself.\",\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"users\": {\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    },\n    \"webhooks\": {\n      \"$ref\": \"#/components/schemas/LinksElement\"\n    }\n  },\n  \"required\": [\n    \"self\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-company-links-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CompanyLinks
---
