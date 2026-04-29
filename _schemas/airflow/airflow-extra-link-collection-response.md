---
description: Extra Links Response.
layout: schema
name: ExtraLinkCollectionResponse
properties_list:
- description: ''
  name: extra_links
  type: object
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-extra-link-collection-response-schema.json
slug: airflow-extra-link-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-extra-link-collection-response-schema.json\",\n  \"title\": \"ExtraLinkCollectionResponse\",\n  \"description\": \"Extra Links Response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"extra_links\": {\n      \"additionalProperties\": {\n        \"anyOf\": [\n          {\n            \"type\": \"string\"\n          },\n          {\n            \"type\": \"null\"\n          }\n        ]\n      },\n      \"type\": \"object\",\n      \"title\": \"Extra Links\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"extra_links\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-extra-link-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ExtraLinkCollectionResponse
---
