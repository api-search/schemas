---
description: PartitionField schema from Apache Iceberg REST Catalog API
layout: schema
name: PartitionField
properties_list:
- description: ''
  name: field-id
  type: integer
- description: ''
  name: source-id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: transform
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-partition-field-schema.json
slug: rest-catalog-open-api-partition-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-partition-field-schema.json\",\n  \"title\": \"PartitionField\",\n  \"description\": \"PartitionField schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field-id\": {\n      \"type\": \"integer\"\n    },\n    \"source-id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"transform\": {\n      \"$ref\": \"#/components/schemas/Transform\"\n    }\n  },\n  \"required\": [\n    \"source-id\",\n    \"transform\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-partition-field-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: PartitionField
---
