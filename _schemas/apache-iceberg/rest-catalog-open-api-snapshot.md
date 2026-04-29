---
description: Snapshot schema from Apache Iceberg REST Catalog API
layout: schema
name: Snapshot
properties_list:
- description: ''
  name: snapshot-id
  type: integer
- description: ''
  name: parent-snapshot-id
  type: integer
- description: ''
  name: sequence-number
  type: integer
- description: ''
  name: timestamp-ms
  type: integer
- description: Location of the snapshot's manifest list file
  name: manifest-list
  type: string
- description: The first _row_id assigned to the first row in the first data file in the first manifest
  name: first-row-id
  type: integer
- description: The upper bound of the number of rows with assigned row IDs
  name: added-rows
  type: integer
- description: ''
  name: summary
  type: object
- description: ''
  name: schema-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-snapshot-schema.json
slug: rest-catalog-open-api-snapshot
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-snapshot-schema.json\",\n  \"title\": \"Snapshot\",\n  \"description\": \"Snapshot schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"parent-snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"sequence-number\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"timestamp-ms\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"manifest-list\": {\n      \"type\": \"string\",\n      \"description\": \"Location of the snapshot's manifest list file\"\n    },\n    \"first-row-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\"\
  : \"The first _row_id assigned to the first row in the first data file in the first manifest\"\n    },\n    \"added-rows\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The upper bound of the number of rows with assigned row IDs\"\n    },\n    \"summary\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"operation\"\n      ],\n      \"properties\": {\n        \"operation\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"append\",\n            \"replace\",\n            \"overwrite\",\n            \"delete\"\n          ]\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"schema-id\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"snapshot-id\",\n    \"timestamp-ms\",\n    \"manifest-list\",\n    \"summary\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-snapshot-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: Snapshot
---
