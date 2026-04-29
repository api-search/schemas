---
description: It conveys the result of the Enable Service processing. Content of the Enable Service Response message.
layout: schema
name: EnableServiceResponse
properties_list:
- description: ''
  name: Response
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-enable-service-response-schema.json
slug: terminal-enable-service-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-enable-service-response-schema.json\",\n  \"title\": \"EnableServiceResponse\",\n  \"description\": \"It conveys the result of the Enable Service processing. Content of the Enable Service Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    }\n  },\n  \"required\": [\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-enable-service-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: EnableServiceResponse
---
