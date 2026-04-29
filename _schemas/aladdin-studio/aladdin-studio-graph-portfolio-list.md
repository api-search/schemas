---
description: Paginated list of portfolios
layout: schema
name: PortfolioList
properties_list:
- description: Array of portfolio objects
  name: portfolios
  type: array
- description: Total number of portfolios
  name: totalCount
  type: integer
- description: Current page number
  name: page
  type: integer
- description: Number of results per page
  name: pageSize
  type: integer
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-graph-portfolio-list-schema.json
slug: aladdin-studio-graph-portfolio-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-portfolio-list-schema.json\",\n  \"title\": \"PortfolioList\",\n  \"description\": \"Paginated list of portfolios\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portfolios\": {\n      \"type\": \"array\",\n      \"description\": \"Array of portfolio objects\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Portfolio\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of portfolios\",\n      \"example\": 125\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\",\n      \"example\": 1\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results per page\",\n      \"example\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-portfolio-list-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: PortfolioList
---
