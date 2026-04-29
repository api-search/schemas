---
description: ''
layout: schema
name: Glue
properties_list:
- description: ARN for AWS role to assume
  name: glue_aws_role_arn
  type: string
- description: Glue catalog id
  name: glue_catalog_id
  type: string
- description: AWS region of the Glue catalog. Must be specified if the Snowflake account is not hosted on AWS.
  name: glue_region
  type: string
- description: default AWS Glue catalog namespace for all Iceberg table that use this catalog integration
  name: catalog_namespace
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/catalog-integration-glue-schema.json
slug: catalog-integration-glue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Glue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"glue_aws_role_arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN for AWS role to assume\"\n    },\n    \"glue_catalog_id\": {\n      \"type\": \"string\",\n      \"description\": \"Glue catalog id\"\n    },\n    \"glue_region\": {\n      \"type\": \"string\",\n      \"description\": \"AWS region of the Glue catalog. Must be specified if the Snowflake account is not hosted on AWS.\"\n    },\n    \"catalog_namespace\": {\n      \"type\": \"string\",\n      \"description\": \"default AWS Glue catalog namespace for all Iceberg table that use this catalog integration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/catalog-integration-glue-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Glue
---
