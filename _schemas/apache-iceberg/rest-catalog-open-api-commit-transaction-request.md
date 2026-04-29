---
description: CommitTransactionRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: CommitTransactionRequest
properties_list:
- description: ''
  name: table-changes
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-commit-transaction-request-schema.json
slug: rest-catalog-open-api-commit-transaction-request
source_filename: rest-catalog-open-api-commit-transaction-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-commit-transaction-request-schema.json\",\n  \"title\": \"CommitTransactionRequest\",\n  \"description\": \"CommitTransactionRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"table-changes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"description\": \"Table commit request; must provide an `identifier`\",\n        \"$ref\": \"#/components/schemas/CommitTableRequest\"\n      }\n    }\n  },\n  \"required\": [\n    \"table-changes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-commit-transaction-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CommitTransactionRequest
---
