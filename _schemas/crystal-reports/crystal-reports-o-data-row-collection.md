---
description: A collection of OData report data rows
layout: schema
name: ODataRowCollection
properties_list:
- description: Total count of rows (when $inlinecount=allpages is used)
  name: __count
  type: string
- description: URI for the next page of results
  name: __next
  type: string
- description: Array of data rows
  name: value
  type: array
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-o-data-row-collection-schema.json
slug: crystal-reports-o-data-row-collection
source_filename: crystal-reports-o-data-row-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-o-data-row-collection-schema.json\",\n  \"title\": \"ODataRowCollection\",\n  \"description\": \"A collection of OData report data rows\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"__count\": {\n      \"type\": \"string\",\n      \"description\": \"Total count of rows (when $inlinecount=allpages is used)\",\n      \"example\": \"1542\"\n    },\n    \"__next\": {\n      \"type\": \"string\",\n      \"description\": \"URI for the next page of results\",\n      \"example\": \"/biprws/infostore/5765/rpt/data.svc/Rows?$skiptoken=100\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"Array of data rows\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ODataRow\"\n      },\n      \"example\": [\n        {\n          \"CustomerName\": \"\
  City Cyclists\",\n          \"Country\": \"USA\",\n          \"OrderAmount\": 1250.5,\n          \"OrderDate\": \"2023-11-15\"\n        },\n        {\n          \"CustomerName\": \"Pathfinders\",\n          \"Country\": \"Canada\",\n          \"OrderAmount\": 875.25,\n          \"OrderDate\": \"2023-11-16\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-o-data-row-collection-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: ODataRowCollection
---
