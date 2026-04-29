---
description: Individual owning the merchant.
layout: schema
name: BeneficialOwner
properties_list:
- description: Beneficial owner birth date. Date must be in a [ISO 8601 format](https://datatracker.ietf.org/doc/html/rfc3339#section-5.6)
  name: birthDate
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-beneficial-owner-schema.json
slug: mastercard-ethoca-merchant-self-services-beneficial-owner
source_filename: mastercard-ethoca-merchant-self-services-beneficial-owner-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BeneficialOwner\",\n  \"type\": \"object\",\n  \"description\": \"Individual owning the merchant.\",\n  \"properties\": {\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficial owner birth date. Date must be in a [ISO 8601 format](https://datatracker.ietf.org/doc/html/rfc3339#section-5.6)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-beneficial-owner-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: BeneficialOwner
---
