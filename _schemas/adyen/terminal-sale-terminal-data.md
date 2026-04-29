---
description: In the Login Request, if a Sale Terminal is involved in the login. In other messages, when a logical device is out of order (SaleCapabilites), or when the other data have changed since or were not in the Login. Information related to the software and hardware feature of the Sale Terminal.
layout: schema
name: SaleTerminalData
properties_list:
- description: If present, default value for all transaction.
  name: TotalsGroupID
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sale-terminal-data-schema.json
slug: terminal-sale-terminal-data
source_filename: terminal-sale-terminal-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-terminal-data-schema.json\",\n  \"title\": \"SaleTerminalData\",\n  \"description\": \"In the Login Request, if a Sale Terminal is involved in the login. In other messages, when a logical device is out of order (SaleCapabilites), or when the other data have changed since or were not in the Login. Information related to the software and hardware feature of the Sale Terminal.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TotalsGroupID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.{1,16}$\",\n      \"description\": \"If present, default value for all transaction.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-terminal-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SaleTerminalData
---
