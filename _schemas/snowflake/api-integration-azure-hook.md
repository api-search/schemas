---
description: ''
layout: schema
name: AzureHook
properties_list:
- description: ''
  name: api_provider
  type: string
- description: The ID of the Office 365 tenant that all Azure API Management instances belong to.
  name: azure_tenant_id
  type: string
- description: The application ID of the Azure Active Directory application.
  name: azure_ad_application_id
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/api-integration-azure-hook-schema.json
slug: api-integration-azure-hook
source_filename: api-integration-azure-hook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AzureHook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api_provider\": {\n      \"type\": \"string\"\n    },\n    \"azure_tenant_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Office 365 tenant that all Azure API Management instances belong to.\"\n    },\n    \"azure_ad_application_id\": {\n      \"type\": \"string\",\n      \"description\": \"The application ID of the Azure Active Directory application.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/api-integration-azure-hook-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: AzureHook
---
