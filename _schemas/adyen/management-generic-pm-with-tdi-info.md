---
description: GenericPmWithTdiInfo schema from Adyen API
layout: schema
name: GenericPmWithTdiInfo
properties_list:
- description: Information regarding the transaction description.
  name: transactionDescription
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-generic-pm-with-tdi-info-schema.json
slug: management-generic-pm-with-tdi-info
source_filename: management-generic-pm-with-tdi-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-generic-pm-with-tdi-info-schema.json\",\n  \"title\": \"GenericPmWithTdiInfo\",\n  \"description\": \"GenericPmWithTdiInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionDescription\": {\n      \"description\": \"Information regarding the transaction description.\",\n      \"$ref\": \"#/components/schemas/TransactionDescriptionInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-generic-pm-with-tdi-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GenericPmWithTdiInfo
---
