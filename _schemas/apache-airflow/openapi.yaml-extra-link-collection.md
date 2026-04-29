---
description: The collection of extra links.
layout: schema
name: ExtraLinkCollection
properties_list:
- description: ''
  name: extra_links
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-extra-link-collection-schema.json
slug: openapi.yaml-extra-link-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-extra-link-collection-schema.json\",\n  \"title\": \"ExtraLinkCollection\",\n  \"description\": \"The collection of extra links.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"extra_links\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ExtraLink\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-extra-link-collection-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: ExtraLinkCollection
---
