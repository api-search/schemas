---
description: RegisterTableRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: RegisterTableRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: metadata-location
  type: string
- description: Whether to overwrite table metadata if the table already exists
  name: overwrite
  type: boolean
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-register-table-request-schema.json
slug: rest-catalog-open-api-register-table-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-register-table-request-schema.json\",\n  \"title\": \"RegisterTableRequest\",\n  \"description\": \"RegisterTableRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"metadata-location\": {\n      \"type\": \"string\"\n    },\n    \"overwrite\": {\n      \"description\": \"Whether to overwrite table metadata if the table already exists\",\n      \"type\": \"boolean\",\n      \"default\": false\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"metadata-location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-register-table-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: RegisterTableRequest
---
