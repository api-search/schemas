---
description: Updates to the configuration parameters for the default Amazon Glue database. You use this database for SQL queries that you write in a Kinesis Data Analytics Studio notebook.
layout: schema
name: CatalogConfigurationUpdate
properties_list:
- description: ''
  name: GlueDataCatalogConfigurationUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-catalog-configuration-update-schema.json
slug: amazon-managed-apache-flink-catalog-configuration-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-catalog-configuration-update-schema.json\",\n  \"title\": \"CatalogConfigurationUpdate\",\n  \"description\": \"Updates to the configuration parameters for the default Amazon Glue database. You use this database for SQL queries that you write in a Kinesis Data Analytics Studio notebook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GlueDataCatalogConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueDataCatalogConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Updates to the configuration parameters for the default Amazon Glue database. You use this database for SQL queries that you write in a Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"GlueDataCatalogConfigurationUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-catalog-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CatalogConfigurationUpdate
---
