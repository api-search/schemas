---
description: Result of server-side scan planning for fetchPlanningResult
layout: schema
name: FetchPlanningResult
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-fetch-planning-result-schema.json
slug: rest-catalog-open-api-fetch-planning-result
source_filename: rest-catalog-open-api-fetch-planning-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-fetch-planning-result-schema.json\",\n  \"title\": \"FetchPlanningResult\",\n  \"description\": \"Result of server-side scan planning for fetchPlanningResult\",\n  \"type\": \"object\",\n  \"oneOf\": [\n    {\n      \"$ref\": \"#/components/schemas/CompletedPlanningResult\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/FailedPlanningResult\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/EmptyPlanningResult\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-fetch-planning-result-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: FetchPlanningResult
---
