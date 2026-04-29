---
description: It conveys Information related to the Login to process. Content of the Login Response message.
layout: schema
name: LoginResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: ''
  name: POISystemData
  type: object
- description: ''
  name: TokenRequestStatus
  type: boolean
- description: ''
  name: CustomerOrderStatus
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-login-response-schema.json
slug: terminal-login-response
source_filename: terminal-login-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-login-response-schema.json\",\n  \"title\": \"LoginResponse\",\n  \"description\": \"It conveys Information related to the Login to process. Content of the Login Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"POISystemData\": {\n      \"$ref\": \"#/components/schemas/POISystemData\"\n    },\n    \"TokenRequestStatus\": {\n      \"type\": \"boolean\"\n    },\n    \"CustomerOrderStatus\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-login-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoginResponse
---
