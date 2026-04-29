---
description: ''
layout: schema
name: DescribeTableResponse
properties_list:
- description: The name of the table
  name: TableName
  type: string
- description: List of column definitions for the table
  name: ColumnList
  type: array
- description: Pagination token for the next page
  name: NextToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-describe-table-response-schema.json
slug: amazon-redshift-data-describe-table-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeTableResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table\"\n    },\n    \"ColumnList\": {\n      \"type\": \"array\",\n      \"description\": \"List of column definitions for the table\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-describe-table-response-schema.json
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
title: DescribeTableResponse
---
