---
description: An on-premises data gateway
layout: schema
name: Gateway
properties_list:
- description: The unique identifier of the gateway
  name: id
  type: string
- description: The display name of the gateway
  name: name
  type: string
- description: The type of gateway
  name: type
  type: string
- description: The public key for encrypting credentials
  name: publicKey
  type: object
- description: Gateway metadata annotation
  name: gatewayAnnotation
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-gateway-schema.json
slug: power-bi-rest-gateway
source_filename: power-bi-rest-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Gateway\",\n  \"type\": \"object\",\n  \"description\": \"An on-premises data gateway\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the gateway\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the gateway\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of gateway\"\n    },\n    \"publicKey\": {\n      \"type\": \"object\",\n      \"description\": \"The public key for encrypting credentials\"\n    },\n    \"gatewayAnnotation\": {\n      \"type\": \"string\",\n      \"description\": \"Gateway metadata annotation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-gateway-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Gateway
---
