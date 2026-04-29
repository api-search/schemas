---
description: ''
layout: schema
name: ListDatabasesResponse
properties_list:
- description: List of database names
  name: Databases
  type: array
- description: Pagination token for the next page
  name: NextToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-list-databases-response-schema.json
slug: amazon-redshift-data-list-databases-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListDatabasesResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Databases\": {\n      \"type\": \"array\",\n      \"description\": \"List of database names\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-list-databases-response-schema.json
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
title: ListDatabasesResponse
---
