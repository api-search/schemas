---
description: Provider serializer for responses.
layout: schema
name: ProviderResponse
properties_list:
- description: ''
  name: package_name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: documentation_url
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-provider-response-schema.json
slug: airflow-provider-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-provider-response-schema.json\",\n  \"title\": \"ProviderResponse\",\n  \"description\": \"Provider serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"package_name\": {\n      \"type\": \"string\",\n      \"title\": \"Package Name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"title\": \"Description\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"title\": \"Version\"\n    },\n    \"documentation_url\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Documentation Url\"\n    }\n  },\n  \"required\": [\n    \"package_name\",\n    \"description\",\n    \"version\",\n    \"documentation_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-provider-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ProviderResponse
---
