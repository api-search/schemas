---
description: Schema schema from Apache Iceberg REST Catalog API
layout: schema
name: Schema
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-schema-schema.json
slug: rest-catalog-open-api-schema
source_filename: rest-catalog-open-api-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-schema-schema.json\",\n  \"title\": \"Schema\",\n  \"description\": \"Schema schema from Apache Iceberg REST Catalog API\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/StructType\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"schema-id\": {\n          \"type\": \"integer\",\n          \"readOnly\": true\n        },\n        \"identifier-field-ids\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-schema-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: Schema
---
