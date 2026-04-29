---
description: It conveys the result of the Logout. Content of the Logout Response message.
layout: schema
name: LogoutResponse
properties_list:
- description: ''
  name: Response
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-logout-response-schema.json
slug: terminal-logout-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-logout-response-schema.json\",\n  \"title\": \"LogoutResponse\",\n  \"description\": \"It conveys the result of the Logout. Content of the Logout Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    }\n  },\n  \"required\": [\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-logout-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LogoutResponse
---
