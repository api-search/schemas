---
description: It conveys information from the Sale System related to the scope and the format of the totals to be computed by the POI System. Content of the Get Totals Request message.
layout: schema
name: GetTotalsRequest
properties_list:
- description: ''
  name: TotalDetails
  type: object
- description: ''
  name: TotalFilter
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-get-totals-request-schema.json
slug: terminal-get-totals-request
source_filename: terminal-get-totals-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-get-totals-request-schema.json\",\n  \"title\": \"GetTotalsRequest\",\n  \"description\": \"It conveys information from the Sale System related to the scope and the format of the totals to be computed by the POI System. Content of the Get Totals Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TotalDetails\": {\n      \"$ref\": \"#/components/schemas/TotalDetails\"\n    },\n    \"TotalFilter\": {\n      \"$ref\": \"#/components/schemas/TotalFilter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-get-totals-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetTotalsRequest
---
