---
description: PartitionSpec schema from Apache Iceberg REST Catalog API
layout: schema
name: PartitionSpec
properties_list:
- description: ''
  name: spec-id
  type: integer
- description: ''
  name: fields
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-partition-spec-schema.json
slug: rest-catalog-open-api-partition-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-partition-spec-schema.json\",\n  \"title\": \"PartitionSpec\",\n  \"description\": \"PartitionSpec schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spec-id\": {\n      \"type\": \"integer\",\n      \"readOnly\": true\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PartitionField\"\n      }\n    }\n  },\n  \"required\": [\n    \"fields\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-partition-spec-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: PartitionSpec
---
