---
description: Failed server-side planning result
layout: schema
name: FailedPlanningResult
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-failed-planning-result-schema.json
slug: rest-catalog-open-api-failed-planning-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-failed-planning-result-schema.json\",\n  \"title\": \"FailedPlanningResult\",\n  \"description\": \"Failed server-side planning result\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/IcebergErrorResponse\"\n    },\n    {\n      \"type\": \"object\",\n      \"required\": [\n        \"status\"\n      ],\n      \"properties\": {\n        \"status\": {\n          \"$ref\": \"#/components/schemas/PlanStatus\",\n          \"const\": \"failed\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-failed-planning-result-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: FailedPlanningResult
---
