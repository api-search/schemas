---
description: The debug setting.
layout: schema
name: DebugSetting
properties_list:
- description: Specifies the type of information to log for debugging. The permitted values are none, requestContent, responseContent, or both.
  name: detailLevel
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-debug-setting-schema.json
slug: azure-resource-manager-debug-setting
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DebugSetting\",\n  \"type\": \"object\",\n  \"description\": \"The debug setting.\",\n  \"properties\": {\n    \"detailLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the type of information to log for debugging. The permitted values are none, requestContent, responseContent, or both.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-debug-setting-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: DebugSetting
---
