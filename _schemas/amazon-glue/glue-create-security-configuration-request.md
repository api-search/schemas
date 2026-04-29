---
description: CreateSecurityConfigurationRequest schema from Amazon Glue API
layout: schema
name: CreateSecurityConfigurationRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-security-configuration-request-schema.json
slug: glue-create-security-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-security-configuration-request-schema.json\",\n  \"title\": \"CreateSecurityConfigurationRequest\",\n  \"description\": \"CreateSecurityConfigurationRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name for the new security configuration.\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n        {\n          \"description\": \"The encryption configuration for the new security configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"EncryptionConfiguration\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-security-configuration-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateSecurityConfigurationRequest
---
