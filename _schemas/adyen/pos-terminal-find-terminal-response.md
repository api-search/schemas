---
description: FindTerminalResponse schema from Adyen API
layout: schema
name: FindTerminalResponse
properties_list:
- description: The company account that the terminal is associated with. If this is the only account level shown in the response, the terminal is assigned to the inventory of the company account.
  name: companyAccount
  type: string
- description: The merchant account that the terminal is associated with. If the response doesn't contain a `store` the terminal is assigned to this merchant account.
  name: merchantAccount
  type: string
- description: Boolean that indicates if the terminal is assigned to the merchant inventory. This is returned when the terminal is assigned to a merchant account. - If **true**, this indicates that the terminal is i
  name: merchantInventory
  type: boolean
- description: The store code of the store that the terminal is assigned to.
  name: store
  type: string
- description: The unique terminal ID.
  name: terminal
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-find-terminal-response-schema.json
slug: pos-terminal-find-terminal-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-find-terminal-response-schema.json\",\n  \"title\": \"FindTerminalResponse\",\n  \"description\": \"FindTerminalResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyAccount\": {\n      \"description\": \"The company account that the terminal is associated with. If this is the only account level shown in the response, the terminal is assigned to the inventory of the company account.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that the terminal is associated with. If the response doesn't contain a `store` the terminal is assigned to this merchant account.\",\n      \"type\": \"string\"\n    },\n    \"merchantInventory\": {\n      \"description\": \"Boolean that indicates if the terminal is assigned\
  \ to the merchant inventory. This is returned when the terminal is assigned to a merchant account.\\n\\n- If **true**, this indicates that the terminal is in the merchant inventory. This also means that the terminal cannot be boarded.\\n\\n- If **false**, this indicates that the terminal is assigned to the merchant account as an in-store terminal. This means that the terminal is ready to be boarded, or is already boarded.\",\n      \"type\": \"boolean\"\n    },\n    \"store\": {\n      \"description\": \"The store code of the store that the terminal is assigned to.\",\n      \"type\": \"string\"\n    },\n    \"terminal\": {\n      \"description\": \"The unique terminal ID.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"companyAccount\",\n    \"terminal\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-find-terminal-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: FindTerminalResponse
---
