---
description: CommitTableResponse schema from Apache Iceberg REST Catalog API
layout: schema
name: CommitTableResponse
properties_list:
- description: ''
  name: metadata-location
  type: string
- description: ''
  name: metadata
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-commit-table-response-schema.json
slug: rest-catalog-open-api-commit-table-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-commit-table-response-schema.json\",\n  \"title\": \"CommitTableResponse\",\n  \"description\": \"CommitTableResponse schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata-location\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/components/schemas/TableMetadata\"\n    }\n  },\n  \"required\": [\n    \"metadata-location\",\n    \"metadata\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-commit-table-response-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CommitTableResponse
---
