---
description: UpdatableAddress schema from Adyen API
layout: schema
name: UpdatableAddress
properties_list:
- description: The name of the city.
  name: city
  type: string
- description: The street address.
  name: line1
  type: string
- description: Second address line.
  name: line2
  type: string
- description: Third address line.
  name: line3
  type: string
- description: The postal code.
  name: postalCode
  type: string
- description: 'The state or province code as defined in [ISO 3166-2](https://www.iso.org/standard/72483.html). For example, **ON** for Ontario, Canada. Required for the following countries: - Australia - Brazil - Ca'
  name: stateOrProvince
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-updatable-address-schema.json
slug: management-updatable-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-updatable-address-schema.json\",\n  \"title\": \"UpdatableAddress\",\n  \"description\": \"UpdatableAddress schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"description\": \"The name of the city.\",\n      \"type\": \"string\"\n    },\n    \"line1\": {\n      \"description\": \"The street address.\",\n      \"type\": \"string\"\n    },\n    \"line2\": {\n      \"description\": \"Second address line.\",\n      \"type\": \"string\"\n    },\n    \"line3\": {\n      \"description\": \"Third address line.\",\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"description\": \"The postal code.\",\n      \"type\": \"string\"\n    },\n    \"stateOrProvince\": {\n      \"description\": \"The state or province code as defined in [ISO 3166-2](https://www.iso.org/standard/72483.html).\
  \ For example, **ON** for Ontario, Canada.\\n\\nRequired for the following countries:\\n - Australia\\n- Brazil\\n- Canada\\n- India\\n- Mexico\\n- New Zealand\\n- United States\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-updatable-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdatableAddress
---
