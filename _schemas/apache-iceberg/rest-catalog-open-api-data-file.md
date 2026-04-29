---
description: DataFile schema from Apache Iceberg REST Catalog API
layout: schema
name: DataFile
properties_list:
- description: ''
  name: content
  type: string
- description: The first row ID assigned to the first row in the data file
  name: first-row-id
  type: integer
- description: Map of column id to total count, including null and NaN
  name: column-sizes
  type: object
- description: Map of column id to null value count
  name: value-counts
  type: object
- description: Map of column id to null value count
  name: null-value-counts
  type: object
- description: Map of column id to number of NaN values in the column
  name: nan-value-counts
  type: object
- description: Map of column id to lower bound primitive type values
  name: lower-bounds
  type: object
- description: Map of column id to upper bound primitive type values
  name: upper-bounds
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-data-file-schema.json
slug: rest-catalog-open-api-data-file
source_filename: rest-catalog-open-api-data-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-data-file-schema.json\",\n  \"title\": \"DataFile\",\n  \"description\": \"DataFile schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\",\n      \"const\": \"data\"\n    },\n    \"first-row-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The first row ID assigned to the first row in the data file\"\n    },\n    \"column-sizes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountMap\"\n        }\n      ],\n      \"description\": \"Map of column id to total count, including null and NaN\"\n    },\n    \"value-counts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountMap\"\n        }\n  \
  \    ],\n      \"description\": \"Map of column id to null value count\"\n    },\n    \"null-value-counts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountMap\"\n        }\n      ],\n      \"description\": \"Map of column id to null value count\"\n    },\n    \"nan-value-counts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountMap\"\n        }\n      ],\n      \"description\": \"Map of column id to number of NaN values in the column\"\n    },\n    \"lower-bounds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueMap\"\n        }\n      ],\n      \"description\": \"Map of column id to lower bound primitive type values\"\n    },\n    \"upper-bounds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueMap\"\n        }\n      ],\n      \"description\": \"Map of column id to upper bound primitive type values\"\n    }\n  },\n  \"required\": [\n    \"content\"\
  \n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/ContentFile\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-data-file-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: DataFile
---
