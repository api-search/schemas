---
description: WebDataExemption schema from Adyen API
layout: schema
name: WebDataExemption
properties_list:
- description: 'The reason why the web data was not provided. Possible value: **noOnlinePresence**.'
  name: reason
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-web-data-exemption-schema.json
slug: legal-entity-web-data-exemption
source_filename: legal-entity-web-data-exemption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-web-data-exemption-schema.json\",\n  \"title\": \"WebDataExemption\",\n  \"description\": \"WebDataExemption schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reason\": {\n      \"description\": \"The reason why the web data was not provided. Possible value: **noOnlinePresence**.\",\n      \"enum\": [\n        \"noOnlinePresence\",\n        \"notCollectedDuringOnboarding\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-web-data-exemption-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: WebDataExemption
---
