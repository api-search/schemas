---
description: GetSecurityConfigurationResponse schema from Amazon Glue API
layout: schema
name: GetSecurityConfigurationResponse
properties_list:
- description: ''
  name: SecurityConfiguration
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-security-configuration-response-schema.json
slug: glue-get-security-configuration-response
source_filename: glue-get-security-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-security-configuration-response-schema.json\",\n  \"title\": \"GetSecurityConfigurationResponse\",\n  \"description\": \"GetSecurityConfigurationResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecurityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityConfiguration\"\n        },\n        {\n          \"description\": \"The requested security configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-security-configuration-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetSecurityConfigurationResponse
---
