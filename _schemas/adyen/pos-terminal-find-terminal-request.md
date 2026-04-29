---
description: FindTerminalRequest schema from Adyen API
layout: schema
name: FindTerminalRequest
properties_list:
- description: The unique terminal ID in the format `[Device model]-[Serial number]`. For example, **V400m-324689776**.
  name: terminal
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-find-terminal-request-schema.json
slug: pos-terminal-find-terminal-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-find-terminal-request-schema.json\",\n  \"title\": \"FindTerminalRequest\",\n  \"description\": \"FindTerminalRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"terminal\": {\n      \"description\": \"The unique terminal ID in the format `[Device model]-[Serial number]`. \\n\\nFor example, **V400m-324689776**.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"terminal\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-find-terminal-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: FindTerminalRequest
---
