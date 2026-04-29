---
description: OwnerEntity schema from Adyen API
layout: schema
name: OwnerEntity
properties_list:
- description: Unique identifier of the resource that owns the document. For `type` **legalEntity**, this value is the unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/p
  name: id
  type: string
- description: 'Type of resource that owns the document. Possible values: **legalEntity**, **bankAccount**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-owner-entity-schema.json
slug: legal-entity-owner-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-owner-entity-schema.json\",\n  \"title\": \"OwnerEntity\",\n  \"description\": \"OwnerEntity schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the resource that owns the document. For `type` **legalEntity**, this value is the unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id). For `type` **bankAccount**, this value is the unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/legalentity/latest/post/transferInstruments#responses-200-id).\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of resource that owns the document.\\n\\nPossible values: **legalEntity**, **bankAccount**.\"\
  ,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-owner-entity-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OwnerEntity
---
