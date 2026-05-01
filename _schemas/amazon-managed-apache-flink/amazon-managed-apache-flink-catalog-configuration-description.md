---
description: The configuration parameters for the default Amazon Glue database. You use this database for Apache Flink SQL queries and table API transforms that you write in a Kinesis Data Analytics Studio notebook.
layout: schema
name: CatalogConfigurationDescription
properties_list:
- description: ''
  name: GlueDataCatalogConfigurationDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-catalog-configuration-description-schema.json
slug: amazon-managed-apache-flink-catalog-configuration-description
source_filename: amazon-managed-apache-flink-catalog-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-catalog-configuration-description-schema.json\",\n  \"title\": \"CatalogConfigurationDescription\",\n  \"description\": \"The configuration parameters for the default Amazon Glue database. You use this database for Apache Flink SQL queries and table API transforms that you write in a Kinesis Data Analytics Studio notebook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GlueDataCatalogConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueDataCatalogConfigurationDescription\"\n        },\n        {\n          \"description\": \"The configuration parameters for the default Amazon Glue database. You use this database for SQL queries that you write in a Kinesis Data Analytics Studio notebook.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"GlueDataCatalogConfigurationDescription\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-catalog-configuration-description-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CatalogConfigurationDescription
---
