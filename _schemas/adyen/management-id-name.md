---
description: IdName schema from Adyen API
layout: schema
name: IdName
properties_list:
- description: The identifier of the terminal model.
  name: id
  type: string
- description: The name of the terminal model.
  name: name
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-id-name-schema.json
slug: management-id-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-id-name-schema.json\",\n  \"title\": \"IdName\",\n  \"description\": \"IdName schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The identifier of the terminal model.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the terminal model.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-id-name-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: IdName
---
