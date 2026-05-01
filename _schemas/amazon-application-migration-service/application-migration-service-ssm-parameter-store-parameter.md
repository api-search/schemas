---
description: SSM Parameter Store parameter reference
layout: schema
name: SsmParameterStoreParameter
properties_list:
- description: Parameter name
  name: parameterName
  type: string
- description: Parameter type
  name: parameterType
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-ssm-parameter-store-parameter-schema.json
slug: application-migration-service-ssm-parameter-store-parameter
source_filename: application-migration-service-ssm-parameter-store-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-ssm-parameter-store-parameter-schema.json\",\n  \"title\": \"SsmParameterStoreParameter\",\n  \"description\": \"SSM Parameter Store parameter reference\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameterName\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter name\"\n    },\n    \"parameterType\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-ssm-parameter-store-parameter-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: SsmParameterStoreParameter
---
