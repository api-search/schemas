---
description: DisableResult schema from Adyen API
layout: schema
name: DisableResult
properties_list:
- description: Depending on whether a specific recurring detail was in the request, result is either [detail-successfully-disabled] or [all-details-successfully-disabled].
  name: response
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-disable-result-schema.json
slug: recurring-disable-result
source_filename: recurring-disable-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-disable-result-schema.json\",\n  \"title\": \"DisableResult\",\n  \"description\": \"DisableResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"response\": {\n      \"description\": \"Depending on whether a specific recurring detail was in the request, result is either [detail-successfully-disabled] or [all-details-successfully-disabled].\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-disable-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DisableResult
---
