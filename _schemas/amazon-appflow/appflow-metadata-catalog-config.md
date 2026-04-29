---
description: MetadataCatalogConfig schema from Amazon AppFlow API
layout: schema
name: MetadataCatalogConfig
properties_list:
- description: Specifies the configuration that Amazon AppFlow uses when it catalogs data with the Glue Data Catalog.
  name: glueDataCatalog
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-metadata-catalog-config-schema.json
slug: appflow-metadata-catalog-config
source_filename: appflow-metadata-catalog-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-metadata-catalog-config-schema.json\",\n  \"title\": \"MetadataCatalogConfig\",\n  \"description\": \"MetadataCatalogConfig schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"glueDataCatalog\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"roleArn\": {\n          \"type\": \"string\",\n          \"example\": \"arn:aws:iam::123456789012:role/AppFlowGlueRole\",\n          \"description\": \"The ARN of an IAM role that grants AppFlow the permissions it needs to create Data Catalog tables, databases, and partitions.\"\n        },\n        \"databaseName\": {\n          \"type\": \"string\",\n          \"example\": \"appflow-catalog-db\",\n          \"description\": \"The name of an existing Glue Data Catalog database.\"\n        },\n        \"\
  tablePrefix\": {\n          \"type\": \"string\",\n          \"example\": \"sf_\",\n          \"description\": \"A naming prefix for each Data Catalog table that Amazon AppFlow creates.\"\n        }\n      },\n      \"description\": \"Specifies the configuration that Amazon AppFlow uses when it catalogs data with the Glue Data Catalog.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-metadata-catalog-config-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: MetadataCatalogConfig
---
