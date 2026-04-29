---
description: AssignTerminalsRequest schema from Adyen API
layout: schema
name: AssignTerminalsRequest
properties_list:
- description: Your company account. To return terminals to the company inventory, specify only this parameter and the `terminals`.
  name: companyAccount
  type: string
- description: Name of the merchant account. Specify this parameter to assign terminals to this merchant account or to a store under this merchant account.
  name: merchantAccount
  type: string
- description: Boolean that indicates if you are assigning the terminals to the merchant inventory. Do not use when assigning terminals to a store. Required when assigning the terminal to a merchant account. - Set t
  name: merchantInventory
  type: boolean
- description: The store code of the store that you want to assign the terminals to.
  name: store
  type: string
- description: Array containing a list of terminal IDs that you want to assign or reassign to the merchant account or store, or that you want to return to the company inventory. For example, `["V400m-324689776","P40
  name: terminals
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-assign-terminals-request-schema.json
slug: pos-terminal-assign-terminals-request
source_filename: pos-terminal-assign-terminals-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-assign-terminals-request-schema.json\",\n  \"title\": \"AssignTerminalsRequest\",\n  \"description\": \"AssignTerminalsRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyAccount\": {\n      \"description\": \"Your company account. To return terminals to the company inventory, specify only this parameter and the `terminals`.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"Name of the merchant account. Specify this parameter to assign terminals to this merchant account or to a store under this merchant account.\",\n      \"type\": \"string\"\n    },\n    \"merchantInventory\": {\n      \"description\": \"Boolean that indicates if you are assigning the terminals to the merchant inventory. Do not use when assigning terminals\
  \ to a store. Required when assigning the terminal to a merchant account.\\n\\n- Set this to **true** to assign the terminals to the merchant inventory. This also means that the terminals cannot be boarded.\\n\\n- Set this to **false** to assign the terminals to the merchant account as in-store terminals. This makes the terminals ready to be boarded and to process payments through the specified merchant account.\",\n      \"type\": \"boolean\"\n    },\n    \"store\": {\n      \"description\": \"The store code of the store that you want to assign the terminals to.\",\n      \"type\": \"string\"\n    },\n    \"terminals\": {\n      \"description\": \"Array containing a list of terminal IDs that you want to assign or reassign to the merchant account or store, or that you want to return to the company inventory.\\n\\nFor example, `[\\\"V400m-324689776\\\",\\\"P400Plus-329127412\\\"]`.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n \
  \ \"required\": [\n    \"companyAccount\",\n    \"terminals\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-assign-terminals-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AssignTerminalsRequest
---
