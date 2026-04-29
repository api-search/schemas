---
description: Empty. Content of the Custom Admin Request message.
layout: schema
name: AdminRequest
properties_list:
- description: Identification of the administrative service to process.
  name: ServiceIdentification
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-admin-request-schema.json
slug: terminal-admin-request
source_filename: terminal-admin-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-admin-request-schema.json\",\n  \"title\": \"AdminRequest\",\n  \"description\": \"Empty. Content of the Custom Admin Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceIdentification\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Identification of the administrative service to process.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-admin-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdminRequest
---
