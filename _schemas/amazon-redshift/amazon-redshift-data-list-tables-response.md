---
description: ''
layout: schema
name: ListTablesResponse
properties_list:
- description: List of tables
  name: Tables
  type: array
- description: Pagination token for the next page
  name: NextToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-list-tables-response-schema.json
slug: amazon-redshift-data-list-tables-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTablesResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tables\": {\n      \"type\": \"array\",\n      \"description\": \"List of tables\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-list-tables-response-schema.json
tags:
- Analytics
- Big Data
- Cloud
- Data Lake
- Data Warehouse
- ETL
- Machine Learning
- Serverless
- SQL
title: ListTablesResponse
---
