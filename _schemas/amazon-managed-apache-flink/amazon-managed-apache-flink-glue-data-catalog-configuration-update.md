---
description: Updates to the configuration of the Glue Data Catalog that you use for SQL queries that you write in a Kinesis Data Analytics Studio notebook.
layout: schema
name: GlueDataCatalogConfigurationUpdate
properties_list:
- description: ''
  name: DatabaseARNUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-glue-data-catalog-configuration-update-schema.json
slug: amazon-managed-apache-flink-glue-data-catalog-configuration-update
source_filename: amazon-managed-apache-flink-glue-data-catalog-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-glue-data-catalog-configuration-update-schema.json\",\n  \"title\": \"GlueDataCatalogConfigurationUpdate\",\n  \"description\": \"Updates to the configuration of the Glue Data Catalog that you use for SQL queries that you write in a Kinesis Data Analytics Studio notebook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatabaseARNUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseARN\"\n        },\n        {\n          \"description\": \"The updated Amazon Resource Name (ARN) of the database.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseARNUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-glue-data-catalog-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: GlueDataCatalogConfigurationUpdate
---
