---
description: CreateSecurityConfigurationResponse schema from Amazon Glue API
layout: schema
name: CreateSecurityConfigurationResponse
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: CreatedTimestamp
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-security-configuration-response-schema.json
slug: glue-create-security-configuration-response
source_filename: glue-create-security-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-security-configuration-response-schema.json\",\n  \"title\": \"CreateSecurityConfigurationResponse\",\n  \"description\": \"CreateSecurityConfigurationResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name assigned to the new security configuration.\"\n        }\n      ]\n    },\n    \"CreatedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampValue\"\n        },\n        {\n          \"description\": \"The time at which the new security configuration was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-security-configuration-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateSecurityConfigurationResponse
---
