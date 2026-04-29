---
description: CommitTableRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: CommitTableRequest
properties_list:
- description: Table identifier to update; must be present for CommitTransactionRequest
  name: identifier
  type: object
- description: ''
  name: requirements
  type: array
- description: ''
  name: updates
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-commit-table-request-schema.json
slug: rest-catalog-open-api-commit-table-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-commit-table-request-schema.json\",\n  \"title\": \"CommitTableRequest\",\n  \"description\": \"CommitTableRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"description\": \"Table identifier to update; must be present for CommitTransactionRequest\",\n      \"$ref\": \"#/components/schemas/TableIdentifier\"\n    },\n    \"requirements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TableRequirement\"\n      }\n    },\n    \"updates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TableUpdate\"\n      }\n    }\n  },\n  \"required\": [\n    \"requirements\",\n    \"updates\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-commit-table-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CommitTableRequest
---
