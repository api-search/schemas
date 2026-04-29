---
description: Logon credentials for authenticating against the BI Platform
layout: schema
name: LogonRequest
properties_list:
- description: Username for authentication
  name: userName
  type: string
- description: Password for the user account
  name: password
  type: string
- description: Authentication type to use
  name: auth
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-logon-request-schema.json
slug: crystal-reports-logon-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-logon-request-schema.json\",\n  \"title\": \"LogonRequest\",\n  \"description\": \"Logon credentials for authenticating against the BI Platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Username for authentication\",\n      \"example\": \"Administrator\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password for the user account\",\n      \"example\": \"P@ssw0rd\"\n    },\n    \"auth\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication type to use\",\n      \"enum\": [\n        \"secEnterprise\",\n        \"secLDAP\",\n        \"secWinAD\",\n        \"secSAPR3\"\n      ],\n      \"example\": \"secEnterprise\"\n    }\n  },\n  \"required\": [\n   \
  \ \"userName\",\n    \"password\",\n    \"auth\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-logon-request-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: LogonRequest
---
