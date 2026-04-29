---
description: ''
layout: schema
name: GetStatementResultResponse
properties_list:
- description: The results of the SQL statement as an array of rows
  name: Records
  type: array
- description: Metadata about the columns in the result set
  name: ColumnMetadata
  type: array
- description: Total number of rows in the result set
  name: TotalNumRows
  type: integer
- description: Pagination token for the next page of results
  name: NextToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-get-statement-result-response-schema.json
slug: amazon-redshift-data-get-statement-result-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetStatementResultResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Records\": {\n      \"type\": \"array\",\n      \"description\": \"The results of the SQL statement as an array of rows\"\n    },\n    \"ColumnMetadata\": {\n      \"type\": \"array\",\n      \"description\": \"Metadata about the columns in the result set\"\n    },\n    \"TotalNumRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of rows in the result set\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-get-statement-result-response-schema.json
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
title: GetStatementResultResponse
---
