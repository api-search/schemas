---
description: ''
layout: schema
name: DescribeStatementRequest
properties_list:
- description: The identifier of the SQL statement to describe. This value is returned by ExecuteStatement or BatchExecuteStatement.
  name: Id
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-describe-statement-request-schema.json
slug: amazon-redshift-data-describe-statement-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeStatementRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the SQL statement to describe. This value is returned by ExecuteStatement or BatchExecuteStatement.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-describe-statement-request-schema.json
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
title: DescribeStatementRequest
---
