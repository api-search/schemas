---
description: DisablePermitRequest schema from Adyen API
layout: schema
name: DisablePermitRequest
properties_list:
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The permit token to disable.
  name: token
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-disable-permit-request-schema.json
slug: recurring-disable-permit-request
source_filename: recurring-disable-permit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-disable-permit-request-schema.json\",\n  \"title\": \"DisablePermitRequest\",\n  \"description\": \"DisablePermitRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"token\": {\n      \"description\": \"The permit token to disable.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"token\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-disable-permit-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DisablePermitRequest
---
