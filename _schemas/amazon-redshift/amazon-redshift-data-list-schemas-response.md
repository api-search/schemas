---
description: ''
layout: schema
name: ListSchemasResponse
properties_list:
- description: List of schema names
  name: Schemas
  type: array
- description: Pagination token for the next page
  name: NextToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-list-schemas-response-schema.json
slug: amazon-redshift-data-list-schemas-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListSchemasResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Schemas\": {\n      \"type\": \"array\",\n      \"description\": \"List of schema names\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-list-schemas-response-schema.json
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
title: ListSchemasResponse
---
