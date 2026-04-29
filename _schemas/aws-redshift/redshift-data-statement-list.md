---
description: StatementList schema from Amazon Redshift
layout: schema
name: StatementList
properties_list: []
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-statement-list-schema.json
slug: redshift-data-statement-list
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"CreatedAt\": {},\n      \"Id\": {},\n      \"IsBatchStatement\": {},\n      \"QueryParameters\": {},\n      \"QueryString\": {},\n      \"QueryStrings\": {},\n      \"SecretArn\": {},\n      \"StatementName\": {},\n      \"Status\": {},\n      \"UpdatedAt\": {}\n    },\n    \"required\": [\n      \"Id\"\n    ],\n    \"description\": \"The SQL statement to run.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-statement-list-schema.json\",\n  \"title\": \"StatementList\",\n  \"description\": \"StatementList schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-statement-list-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: StatementList
---
