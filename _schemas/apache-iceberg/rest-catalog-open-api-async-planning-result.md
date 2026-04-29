---
description: AsyncPlanningResult schema from Apache Iceberg REST Catalog API
layout: schema
name: AsyncPlanningResult
properties_list:
- description: ''
  name: status
  type: object
- description: ID used to track a planning request
  name: plan-id
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-async-planning-result-schema.json
slug: rest-catalog-open-api-async-planning-result
source_filename: rest-catalog-open-api-async-planning-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-async-planning-result-schema.json\",\n  \"title\": \"AsyncPlanningResult\",\n  \"description\": \"AsyncPlanningResult schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"$ref\": \"#/components/schemas/PlanStatus\",\n      \"const\": \"submitted\"\n    },\n    \"plan-id\": {\n      \"description\": \"ID used to track a planning request\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"plan-id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-async-planning-result-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AsyncPlanningResult
---
