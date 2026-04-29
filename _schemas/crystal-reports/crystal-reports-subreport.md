---
description: A subreport embedded within the main report
layout: schema
name: Subreport
properties_list:
- description: Subreport name
  name: name
  type: string
- description: URI to access the subreport
  name: uri
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-subreport-schema.json
slug: crystal-reports-subreport
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-subreport-schema.json\",\n  \"title\": \"Subreport\",\n  \"description\": \"A subreport embedded within the main report\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Subreport name\",\n      \"example\": \"OrderDetails\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI to access the subreport\",\n      \"example\": \"/biprws/infostore/5765/rpt/subreport/OrderDetails\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-subreport-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: Subreport
---
