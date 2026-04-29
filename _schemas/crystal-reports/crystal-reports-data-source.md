---
description: A data source connection used by the report
layout: schema
name: DataSource
properties_list:
- description: Name of the data source
  name: name
  type: string
- description: Type of data source connection
  name: type
  type: string
- description: Tables used from this data source
  name: tables
  type: array
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-data-source-schema.json
slug: crystal-reports-data-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-data-source-schema.json\",\n  \"title\": \"DataSource\",\n  \"description\": \"A data source connection used by the report\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the data source\",\n      \"example\": \"xtreme\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of data source connection\",\n      \"example\": \"JDBC (JNDI)\"\n    },\n    \"tables\": {\n      \"type\": \"array\",\n      \"description\": \"Tables used from this data source\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"Customer\",\n        \"Orders\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-data-source-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: DataSource
---
