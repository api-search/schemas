---
description: Collection of pools. *Changed in version 2.1.0*&#58; 'total_entries' field is added.
layout: schema
name: PoolCollection
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-pool-collection-schema.json
slug: openapi.yaml-pool-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-pool-collection-schema.json\",\n  \"title\": \"PoolCollection\",\n  \"description\": \"Collection of pools.\\n\\n*Changed in version 2.1.0*&#58; 'total_entries' field is added.\\n\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"properties\": {\n        \"pools\": {\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Pool\"\n          },\n          \"type\": \"array\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/CollectionInfo\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-pool-collection-schema.json
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
title: PoolCollection
---
