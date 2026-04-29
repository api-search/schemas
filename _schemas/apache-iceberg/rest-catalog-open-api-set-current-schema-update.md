---
description: SetCurrentSchemaUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: SetCurrentSchemaUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: Schema ID to set as current, or -1 to set last added schema
  name: schema-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-set-current-schema-update-schema.json
slug: rest-catalog-open-api-set-current-schema-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-current-schema-update-schema.json\",\n  \"title\": \"SetCurrentSchemaUpdate\",\n  \"description\": \"SetCurrentSchemaUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"set-current-schema\"\n    },\n    \"schema-id\": {\n      \"type\": \"integer\",\n      \"description\": \"Schema ID to set as current, or -1 to set last added schema\"\n    }\n  },\n  \"required\": [\n    \"schema-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-current-schema-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SetCurrentSchemaUpdate
---
