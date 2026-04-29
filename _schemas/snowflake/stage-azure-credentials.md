---
description: Specifies the Azure credentials of the stage.
layout: schema
name: AzureCredentials
properties_list:
- description: Specifies the SAS (shared access signature) token for connecting to Azure.
  name: azure_sas_token
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stage-azure-credentials-schema.json
slug: stage-azure-credentials
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AzureCredentials\",\n  \"type\": \"object\",\n  \"description\": \"Specifies the Azure credentials of the stage.\",\n  \"properties\": {\n    \"azure_sas_token\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the SAS (shared access signature) token for connecting to Azure.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stage-azure-credentials-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: AzureCredentials
---
