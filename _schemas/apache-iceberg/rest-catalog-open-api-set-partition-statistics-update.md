---
description: SetPartitionStatisticsUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: SetPartitionStatisticsUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: partition-statistics
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-set-partition-statistics-update-schema.json
slug: rest-catalog-open-api-set-partition-statistics-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-partition-statistics-update-schema.json\",\n  \"title\": \"SetPartitionStatisticsUpdate\",\n  \"description\": \"SetPartitionStatisticsUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"set-partition-statistics\"\n    },\n    \"partition-statistics\": {\n      \"$ref\": \"#/components/schemas/PartitionStatisticsFile\"\n    }\n  },\n  \"required\": [\n    \"partition-statistics\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-partition-statistics-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SetPartitionStatisticsUpdate
---
