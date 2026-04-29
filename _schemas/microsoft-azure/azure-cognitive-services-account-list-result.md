---
description: The list of cognitive services accounts.
layout: schema
name: AccountListResult
properties_list:
- description: An array of cognitive services accounts.
  name: value
  type: array
- description: The link used to get the next page of accounts.
  name: nextLink
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-account-list-result-schema.json
slug: azure-cognitive-services-account-list-result
source_filename: azure-cognitive-services-account-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountListResult\",\n  \"type\": \"object\",\n  \"description\": \"The list of cognitive services accounts.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"An array of cognitive services accounts.\"\n    },\n    \"nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The link used to get the next page of accounts.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-account-list-result-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: AccountListResult
---
