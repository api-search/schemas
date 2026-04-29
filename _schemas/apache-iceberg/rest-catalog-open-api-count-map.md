---
description: CountMap schema from Apache Iceberg REST Catalog API
layout: schema
name: CountMap
properties_list:
- description: List of integer column ids for each corresponding value
  name: keys
  type: array
- description: List of Long values, matched to 'keys' by index
  name: values
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-count-map-schema.json
slug: rest-catalog-open-api-count-map
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-count-map-schema.json\",\n  \"title\": \"CountMap\",\n  \"description\": \"CountMap schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/IntegerTypeValue\"\n      },\n      \"description\": \"List of integer column ids for each corresponding value\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LongTypeValue\"\n      },\n      \"description\": \"List of Long values, matched to 'keys' by index\"\n    }\n  },\n  \"example\": {\n    \"keys\": [\n      1,\n      2\n    ],\n    \"values\": [\n      100,\n      200\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-count-map-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CountMap
---
