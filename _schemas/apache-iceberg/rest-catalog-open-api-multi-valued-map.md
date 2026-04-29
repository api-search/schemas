---
description: A map of string keys where each key can map to multiple string values.
layout: schema
name: MultiValuedMap
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-multi-valued-map-schema.json
slug: rest-catalog-open-api-multi-valued-map
source_filename: rest-catalog-open-api-multi-valued-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-multi-valued-map-schema.json\",\n  \"title\": \"MultiValuedMap\",\n  \"description\": \"A map of string keys where each key can map to multiple string values.\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"array\",\n    \"items\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-multi-valued-map-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: MultiValuedMap
---
