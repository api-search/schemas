---
description: ''
layout: schema
name: GetStatementResultRequest
properties_list:
- description: The identifier of the SQL statement whose results to fetch
  name: Id
  type: string
- description: A pagination token for the next page of results
  name: NextToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-get-statement-result-request-schema.json
slug: amazon-redshift-data-get-statement-result-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetStatementResultRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the SQL statement whose results to fetch\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"A pagination token for the next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-get-statement-result-request-schema.json
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
title: GetStatementResultRequest
---
