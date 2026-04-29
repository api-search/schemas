---
description: Request body for creating a stored procedure.
layout: schema
name: StoredProcedureCreateRequest
properties_list:
- description: The unique name of the stored procedure.
  name: id
  type: string
- description: The body of the stored procedure (JavaScript function).
  name: body
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-stored-procedure-create-request-schema.json
slug: azure-cosmos-db-stored-procedure-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StoredProcedureCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a stored procedure.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the stored procedure.\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"The body of the stored procedure (JavaScript function).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-stored-procedure-create-request-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: StoredProcedureCreateRequest
---
