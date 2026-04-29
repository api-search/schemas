---
description: ''
layout: schema
name: ResourceNotFoundException
properties_list:
- description: A description of the resource not found error
  name: Message
  type: string
- description: The identifier of the resource that was not found
  name: ResourceId
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-resource-not-found-exception-schema.json
slug: amazon-redshift-data-resource-not-found-exception
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceNotFoundException\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the resource not found error\"\n    },\n    \"ResourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the resource that was not found\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-resource-not-found-exception-schema.json
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
title: ResourceNotFoundException
---
