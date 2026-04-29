---
description: Response returned when a resource is successfully created
layout: schema
name: ResourceCreatedResponse
properties_list:
- description: The URI of the newly created resource
  name: uri
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-resource-created-response-schema.json
slug: sap-concur-expense-resource-created-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceCreatedResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response returned when a resource is successfully created\",\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI of the newly created resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-resource-created-response-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ResourceCreatedResponse
---
