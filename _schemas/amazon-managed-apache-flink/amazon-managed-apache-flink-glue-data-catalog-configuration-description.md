---
description: The configuration of the Glue Data Catalog that you use for Apache Flink SQL queries and table API transforms that you write in an application.
layout: schema
name: GlueDataCatalogConfigurationDescription
properties_list:
- description: ''
  name: DatabaseARN
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-glue-data-catalog-configuration-description-schema.json
slug: amazon-managed-apache-flink-glue-data-catalog-configuration-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-glue-data-catalog-configuration-description-schema.json\",\n  \"title\": \"GlueDataCatalogConfigurationDescription\",\n  \"description\": \"The configuration of the Glue Data Catalog that you use for Apache Flink SQL queries and table API transforms that you write in an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatabaseARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the database.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-glue-data-catalog-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: GlueDataCatalogConfigurationDescription
---
