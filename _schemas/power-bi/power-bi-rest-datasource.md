---
description: A data source used by a dataset
layout: schema
name: Datasource
properties_list:
- description: The type of data source (e.g. Sql, AnalysisServices, File)
  name: datasourceType
  type: string
- description: Connection details for the data source
  name: connectionDetails
  type: object
- description: The unique identifier of the data source
  name: datasourceId
  type: string
- description: The gateway identifier if using an on-premises gateway
  name: gatewayId
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-datasource-schema.json
slug: power-bi-rest-datasource
source_filename: power-bi-rest-datasource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Datasource\",\n  \"type\": \"object\",\n  \"description\": \"A data source used by a dataset\",\n  \"properties\": {\n    \"datasourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of data source (e.g. Sql, AnalysisServices, File)\"\n    },\n    \"connectionDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Connection details for the data source\"\n    },\n    \"datasourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the data source\"\n    },\n    \"gatewayId\": {\n      \"type\": \"string\",\n      \"description\": \"The gateway identifier if using an on-premises gateway\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-datasource-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Datasource
---
