---
description: Response containing the logon token after successful authentication
layout: schema
name: LogonResponse
properties_list:
- description: Session token for subsequent API calls (include in X-SAP-LogonToken header with quotes)
  name: logonToken
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-logon-response-schema.json
slug: crystal-reports-logon-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-logon-response-schema.json\",\n  \"title\": \"LogonResponse\",\n  \"description\": \"Response containing the logon token after successful authentication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logonToken\": {\n      \"type\": \"string\",\n      \"description\": \"Session token for subsequent API calls (include in X-SAP-LogonToken header with quotes)\",\n      \"example\": \"COMMANDCOM-LCM:6400@{3&2=5697,U3&p=40623.9596541551,Y7&4F&68&z=_3P05,UP&66&UF=02twEaVJw0H1xh3KHPg3S7x.mhc0RWgGLQo1jW.aQbs5Q&42&0F=Ax3kVubd7nkS0DmUxkxGr5J\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-logon-response-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: LogonResponse
---
