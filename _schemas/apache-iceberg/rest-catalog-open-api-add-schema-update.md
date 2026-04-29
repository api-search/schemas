---
description: AddSchemaUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: AddSchemaUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: schema
  type: object
- description: This optional field is **DEPRECATED for REMOVAL** since it more safe to handle this internally, and shouldn't be exposed to the clients. The highest assigned column ID for the table. This is used to e
  name: last-column-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-add-schema-update-schema.json
slug: rest-catalog-open-api-add-schema-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-schema-update-schema.json\",\n  \"title\": \"AddSchemaUpdate\",\n  \"description\": \"AddSchemaUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"add-schema\"\n    },\n    \"schema\": {\n      \"$ref\": \"#/components/schemas/Schema\"\n    },\n    \"last-column-id\": {\n      \"type\": \"integer\",\n      \"deprecated\": true,\n      \"description\": \"This optional field is **DEPRECATED for REMOVAL** since it more safe to handle this internally, and shouldn't be exposed to the clients.\\nThe highest assigned column ID for the table. This is used to ensure columns are always assigned an unused ID when evolving schemas. When omitted, it will be computed on the server side.\"\n    }\n  },\n\
  \  \"required\": [\n    \"schema\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-schema-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AddSchemaUpdate
---
