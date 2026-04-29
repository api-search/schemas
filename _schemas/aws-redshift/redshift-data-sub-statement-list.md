---
description: SubStatementList schema from Amazon Redshift
layout: schema
name: SubStatementList
properties_list: []
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-sub-statement-list-schema.json
slug: redshift-data-sub-statement-list
source_filename: redshift-data-sub-statement-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"CreatedAt\": {},\n      \"Duration\": {},\n      \"Error\": {},\n      \"HasResultSet\": {},\n      \"Id\": {},\n      \"QueryString\": {},\n      \"RedshiftQueryId\": {},\n      \"ResultRows\": {},\n      \"ResultSize\": {},\n      \"Status\": {},\n      \"UpdatedAt\": {}\n    },\n    \"required\": [\n      \"Id\"\n    ],\n    \"description\": \"Information about an SQL statement.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-sub-statement-list-schema.json\",\n  \"title\": \"SubStatementList\",\n  \"description\": \"SubStatementList schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-sub-statement-list-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: SubStatementList
---
