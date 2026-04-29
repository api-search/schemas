---
description: AssignTerminalsResponse schema from Adyen API
layout: schema
name: AssignTerminalsResponse
properties_list:
- description: 'Array that returns a list of the terminals, and for each terminal the result of assigning it to an account or store. The results can be: - `Done`: The terminal has been assigned. - `AssignmentSchedule'
  name: results
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-assign-terminals-response-schema.json
slug: pos-terminal-assign-terminals-response
source_filename: pos-terminal-assign-terminals-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-assign-terminals-response-schema.json\",\n  \"title\": \"AssignTerminalsResponse\",\n  \"description\": \"AssignTerminalsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Array that returns a list of the terminals, and for each terminal the result of assigning it to an account or store.\\n\\nThe results can be: \\n\\n - `Done`: The terminal has been assigned.\\n\\n - `AssignmentScheduled`: The terminal will be assigned asynschronously.\\n\\n - `RemoveConfigScheduled`: The terminal was previously assigned and boarded. Wait for the terminal to synchronize with the Adyen platform. For more information, refer to [Reassigning boarded\\nterminals](https://docs.adyen.com/point-of-sale/managing-terminals/assign-terminals#reassign-boarded-terminals).\\\
  n\\n - `Error`: There was an error when assigning the terminal. \",\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-assign-terminals-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AssignTerminalsResponse
---
