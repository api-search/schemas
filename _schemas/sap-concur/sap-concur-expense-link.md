---
description: A HATEOAS hypermedia link for resource navigation
layout: schema
name: Link
properties_list:
- description: The link relation type
  name: rel
  type: string
- description: The target URI
  name: href
  type: string
- description: Language of the target resource
  name: hreflang
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-link-schema.json
slug: sap-concur-expense-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Link\",\n  \"type\": \"object\",\n  \"description\": \"A HATEOAS hypermedia link for resource navigation\",\n  \"properties\": {\n    \"rel\": {\n      \"type\": \"string\",\n      \"description\": \"The link relation type\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"The target URI\"\n    },\n    \"hreflang\": {\n      \"type\": \"string\",\n      \"description\": \"Language of the target resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-link-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: Link
---
