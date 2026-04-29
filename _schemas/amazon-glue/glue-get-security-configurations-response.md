---
description: GetSecurityConfigurationsResponse schema from Amazon Glue API
layout: schema
name: GetSecurityConfigurationsResponse
properties_list:
- description: ''
  name: SecurityConfigurations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-security-configurations-response-schema.json
slug: glue-get-security-configurations-response
source_filename: glue-get-security-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-security-configurations-response-schema.json\",\n  \"title\": \"GetSecurityConfigurationsResponse\",\n  \"description\": \"GetSecurityConfigurationsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecurityConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityConfigurationList\"\n        },\n        {\n          \"description\": \"A list of security configurations.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if there are more security configurations to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-security-configurations-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetSecurityConfigurationsResponse
---
