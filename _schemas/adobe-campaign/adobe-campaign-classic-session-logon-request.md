---
description: SOAP envelope containing login credentials for session authentication.
layout: schema
name: SessionLogonRequest
properties_list:
- description: Username for authentication.
  name: strLogin
  type: string
- description: Password for authentication.
  name: strPassword
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-session-logon-request-schema.json
slug: adobe-campaign-classic-session-logon-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-session-logon-request-schema.json\",\n  \"title\": \"SessionLogonRequest\",\n  \"description\": \"SOAP envelope containing login credentials for session authentication.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"strLogin\": {\n      \"type\": \"string\",\n      \"description\": \"Username for authentication.\",\n      \"example\": \"example_value\"\n    },\n    \"strPassword\": {\n      \"type\": \"string\",\n      \"description\": \"Password for authentication.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-session-logon-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: SessionLogonRequest
---
