---
description: PermitRestriction schema from Adyen API
layout: schema
name: PermitRestriction
properties_list:
- description: The total sum amount of one or more payments made using this permit may not exceed this amount if set.
  name: maxAmount
  type: object
- description: The amount of any single payment using this permit may not exceed this amount if set.
  name: singleTransactionLimit
  type: object
- description: Only a single payment can be made using this permit if set to true, otherwise multiple payments are allowed.
  name: singleUse
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-permit-restriction-schema.json
slug: recurring-permit-restriction
source_filename: recurring-permit-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-permit-restriction-schema.json\",\n  \"title\": \"PermitRestriction\",\n  \"description\": \"PermitRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxAmount\": {\n      \"description\": \"The total sum amount of one or more payments made using this permit may not exceed this amount if set.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"singleTransactionLimit\": {\n      \"description\": \"The amount of any single payment using this permit may not exceed this amount if set.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"singleUse\": {\n      \"description\": \"Only a single payment can be made using this permit if set to true, otherwise multiple payments are allowed.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-permit-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PermitRestriction
---
