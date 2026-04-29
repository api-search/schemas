---
description: BrandVariantsRestriction schema from Adyen API
layout: schema
name: BrandVariantsRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: 'List of card brand variants. Possible values: - **mc**, **mccredit**, **mccommercialcredit_b2b**, **mcdebit**, **mcbusinessdebit**, **mcbusinessworlddebit**, **mcprepaid**, **mcmaestro** - **visa**, *'
  name: value
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-brand-variants-restriction-schema.json
slug: configuration-brand-variants-restriction
source_filename: configuration-brand-variants-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-brand-variants-restriction-schema.json\",\n  \"title\": \"BrandVariantsRestriction\",\n  \"description\": \"BrandVariantsRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"List of card brand variants.\\n\\nPossible values: \\n\\n- **mc**, **mccredit**, **mccommercialcredit_b2b**, **mcdebit**, **mcbusinessdebit**, **mcbusinessworlddebit**, **mcprepaid**, **mcmaestro**\\n\\n - **visa**, **visacredit**, **visadebit**, **visaprepaid**.\\n\\nYou can specify a rule for a generic variant. For example, to create a rule for all Mastercard payment instruments, use **mc**. The rule is applied to all payment\
  \ instruments under **mc**, such as **mcbusinessdebit** and **mcdebit**.\\n\\n\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-brand-variants-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BrandVariantsRestriction
---
