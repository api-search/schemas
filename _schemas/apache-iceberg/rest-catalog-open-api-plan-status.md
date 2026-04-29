---
description: Status of a server-side planning operation
layout: schema
name: PlanStatus
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-plan-status-schema.json
slug: rest-catalog-open-api-plan-status
source_filename: rest-catalog-open-api-plan-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-plan-status-schema.json\",\n  \"title\": \"PlanStatus\",\n  \"description\": \"Status of a server-side planning operation\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"completed\",\n    \"submitted\",\n    \"cancelled\",\n    \"failed\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-plan-status-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: PlanStatus
---
