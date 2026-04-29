---
description: 'DAG details. For details see: [airflow.models.DAG](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/index.html#airflow.models.DAG)'
layout: schema
name: DAGDetail
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dag-detail-schema.json
slug: openapi.yaml-dag-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-detail-schema.json\",\n  \"title\": \"DAGDetail\",\n  \"description\": \"DAG details.\\n\\nFor details see:\\n[airflow.models.DAG](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/index.html#airflow.models.DAG)\\n\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/DAG\"\n    },\n    {\n      \"properties\": {\n        \"catchup\": {\n          \"readOnly\": true,\n          \"type\": \"boolean\"\n        },\n        \"concurrency\": {\n          \"readOnly\": true,\n          \"type\": \"number\"\n        },\n        \"dag_run_timeout\": {\n          \"$ref\": \"#/components/schemas/TimeDelta\",\n          \"nullable\": true\n        },\n        \"default_view\": {\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n      \
  \  \"doc_md\": {\n          \"nullable\": true,\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"end_date\": {\n          \"description\": \"The DAG's end date.\\n\\n*New in version 2.3.0*.\\n\",\n          \"format\": \"date-time\",\n          \"nullable\": true,\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"is_paused_upon_creation\": {\n          \"description\": \"Whether the DAG is paused upon creation.\\n\\n*New in version 2.3.0*\\n\",\n          \"nullable\": true,\n          \"readOnly\": true,\n          \"type\": \"boolean\"\n        },\n        \"last_parsed\": {\n          \"description\": \"The last time the DAG was parsed.\\n\\n*New in version 2.3.0*\\n\",\n          \"format\": \"date-time\",\n          \"nullable\": true,\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"orientation\": {\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n\
  \        \"params\": {\n          \"description\": \"User-specified DAG params.\\n\\n*New in version 2.0.1*\\n\",\n          \"readOnly\": true,\n          \"type\": \"object\"\n        },\n        \"render_template_as_native_obj\": {\n          \"description\": \"Whether to render templates as native Python objects.\\n\\n*New in version 2.3.0*\\n\",\n          \"nullable\": true,\n          \"readOnly\": true,\n          \"type\": \"boolean\"\n        },\n        \"start_date\": {\n          \"description\": \"The DAG's start date.\\n\\n*Changed in version 2.0.1*&#58; Field becomes nullable.\\n\",\n          \"format\": \"date-time\",\n          \"nullable\": true,\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"template_search_path\": {\n          \"description\": \"The template search path.\\n\\n*New in version 2.3.0*\\n\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"nullable\": true,\n          \"type\"\
  : \"array\"\n        },\n        \"timezone\": {\n          \"$ref\": \"#/components/schemas/Timezone\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-detail-schema.json
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
title: DAGDetail
---
