---
description: Empty server-side planning result
layout: schema
name: EmptyPlanningResult
properties_list:
- description: ''
  name: status
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-empty-planning-result-schema.json
slug: rest-catalog-open-api-empty-planning-result
source_filename: rest-catalog-open-api-empty-planning-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-empty-planning-result-schema.json\",\n  \"title\": \"EmptyPlanningResult\",\n  \"description\": \"Empty server-side planning result\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"$ref\": \"#/components/schemas/PlanStatus\",\n      \"enum\": [\n        \"submitted\",\n        \"cancelled\"\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-empty-planning-result-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: EmptyPlanningResult
---
