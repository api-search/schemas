---
description: A data source on a gateway
layout: schema
name: GatewayDatasource
properties_list:
- description: The unique identifier of the data source
  name: id
  type: string
- description: The gateway this data source belongs to
  name: gatewayId
  type: string
- description: The type of data source
  name: datasourceType
  type: string
- description: JSON string with connection details
  name: connectionDetails
  type: string
- description: The credential type used for authentication
  name: credentialType
  type: string
- description: The display name of the data source
  name: datasourceName
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-gateway-datasource-schema.json
slug: power-bi-rest-gateway-datasource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GatewayDatasource\",\n  \"type\": \"object\",\n  \"description\": \"A data source on a gateway\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the data source\"\n    },\n    \"gatewayId\": {\n      \"type\": \"string\",\n      \"description\": \"The gateway this data source belongs to\"\n    },\n    \"datasourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of data source\"\n    },\n    \"connectionDetails\": {\n      \"type\": \"string\",\n      \"description\": \"JSON string with connection details\"\n    },\n    \"credentialType\": {\n      \"type\": \"string\",\n      \"description\": \"The credential type used for authentication\"\n    },\n    \"datasourceName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the data source\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-gateway-datasource-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: GatewayDatasource
---
