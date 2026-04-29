---
description: Legal entity owning the merchant.
layout: schema
name: LegalEntity
properties_list:
- description: Indicates whether the legal entity is owned by a Government
  name: governmentOwned
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-legal-entity-schema.json
slug: mastercard-ethoca-merchant-self-services-legal-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LegalEntity\",\n  \"type\": \"object\",\n  \"description\": \"Legal entity owning the merchant.\",\n  \"properties\": {\n    \"governmentOwned\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the legal entity is owned by a Government\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-legal-entity-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: LegalEntity
---
