---
description: ''
layout: schema
name: ListStatementsResponse
properties_list:
- description: List of SQL statements
  name: Statements
  type: array
- description: A pagination token to retrieve the next set of results. Null if there are no more results.
  name: NextToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-list-statements-response-schema.json
slug: amazon-redshift-data-list-statements-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListStatementsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Statements\": {\n      \"type\": \"array\",\n      \"description\": \"List of SQL statements\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"A pagination token to retrieve the next set of results. Null if there are no more results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-list-statements-response-schema.json
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
title: ListStatementsResponse
---
