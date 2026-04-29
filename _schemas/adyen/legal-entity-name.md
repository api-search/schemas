---
description: Name schema from Adyen API
layout: schema
name: Name
properties_list:
- description: The individual's first name.
  name: firstName
  type: string
- description: The infix in the individual's name, if any.
  name: infix
  type: string
- description: The individual's last name.
  name: lastName
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-name-schema.json
slug: legal-entity-name
source_filename: legal-entity-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-name-schema.json\",\n  \"title\": \"Name\",\n  \"description\": \"Name schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"description\": \"The individual's first name.\",\n      \"type\": \"string\"\n    },\n    \"infix\": {\n      \"description\": \"The infix in the individual's name, if any.\",\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"The individual's last name.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"firstName\",\n    \"lastName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-name-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Name
---
