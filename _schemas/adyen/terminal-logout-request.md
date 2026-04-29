---
description: Empty. Content of the Logout Request message.
layout: schema
name: LogoutRequest
properties_list:
- description: ''
  name: MaintenanceAllowed
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-logout-request-schema.json
slug: terminal-logout-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-logout-request-schema.json\",\n  \"title\": \"LogoutRequest\",\n  \"description\": \"Empty. Content of the Logout Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaintenanceAllowed\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-logout-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LogoutRequest
---
