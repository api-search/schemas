---
description: CompletedPlanningWithIDResult schema from Apache Iceberg REST Catalog API
layout: schema
name: CompletedPlanningWithIDResult
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-completed-planning-with-id-result-schema.json
slug: rest-catalog-open-api-completed-planning-with-id-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-completed-planning-with-id-result-schema.json\",\n  \"title\": \"CompletedPlanningWithIDResult\",\n  \"description\": \"CompletedPlanningWithIDResult schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/CompletedPlanningResult\"\n    },\n    {\n      \"type\": \"object\",\n      \"required\": [\n        \"plan-id\"\n      ],\n      \"properties\": {\n        \"plan-id\": {\n          \"description\": \"ID used to track a planning request\",\n          \"type\": \"string\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-completed-planning-with-id-result-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CompletedPlanningWithIDResult
---
