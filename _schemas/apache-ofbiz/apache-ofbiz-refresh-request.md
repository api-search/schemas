---
description: Request body for token refresh.
layout: schema
name: RefreshRequest
properties_list:
- description: The refresh token previously issued by /auth/token.
  name: refresh_token
  type: string
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-refresh-request-schema.json
slug: apache-ofbiz-refresh-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-refresh-request-schema.json\",\n  \"title\": \"RefreshRequest\",\n  \"description\": \"Request body for token refresh.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"The refresh token previously issued by /auth/token.\",\n      \"example\": \"dGhpc19pc19hX3JlZnJlc2hfdG9rZW4\"\n    }\n  },\n  \"required\": [\n    \"refresh_token\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-refresh-request-schema.json
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: RefreshRequest
---
