---
description: Trigger rule. *Changed in version 2.2.0*&#58; 'none_failed_min_one_success' is added as a possible value.
layout: schema
name: TriggerRule
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-trigger-rule-schema.json
slug: openapi.yaml-trigger-rule
source_filename: openapi.yaml-trigger-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-trigger-rule-schema.json\",\n  \"title\": \"TriggerRule\",\n  \"description\": \"Trigger rule.\\n\\n*Changed in version 2.2.0*&#58; 'none_failed_min_one_success' is added as a possible value.\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"all_success\",\n    \"all_failed\",\n    \"all_done\",\n    \"one_success\",\n    \"one_failed\",\n    \"none_failed\",\n    \"none_skipped\",\n    \"none_failed_or_skipped\",\n    \"none_failed_min_one_success\",\n    \"dummy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-trigger-rule-schema.json
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
title: TriggerRule
---
