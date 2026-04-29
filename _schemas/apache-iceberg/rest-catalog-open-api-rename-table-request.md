---
description: RenameTableRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: RenameTableRequest
properties_list:
- description: ''
  name: source
  type: object
- description: ''
  name: destination
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-rename-table-request-schema.json
slug: rest-catalog-open-api-rename-table-request
source_filename: rest-catalog-open-api-rename-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-rename-table-request-schema.json\",\n  \"title\": \"RenameTableRequest\",\n  \"description\": \"RenameTableRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"$ref\": \"#/components/schemas/TableIdentifier\"\n    },\n    \"destination\": {\n      \"$ref\": \"#/components/schemas/TableIdentifier\"\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-rename-table-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: RenameTableRequest
---
