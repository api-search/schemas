---
description: CapitalGrants schema from Adyen API
layout: schema
name: CapitalGrants
properties_list:
- description: The unique identifier of the grant.
  name: grants
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-capital-grants-schema.json
slug: transfers-capital-grants
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-capital-grants-schema.json\",\n  \"title\": \"CapitalGrants\",\n  \"description\": \"CapitalGrants schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grants\": {\n      \"description\": \"The unique identifier of the grant.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CapitalGrant\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"grants\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-capital-grants-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapitalGrants
---
