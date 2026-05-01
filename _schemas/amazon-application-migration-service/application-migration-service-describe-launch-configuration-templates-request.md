---
description: Request to describe launch configuration templates
layout: schema
name: DescribeLaunchConfigurationTemplatesRequest
properties_list:
- description: Filter by template IDs
  name: launchConfigurationTemplateIDs
  type: array
- description: Maximum results to return
  name: maxResults
  type: integer
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-describe-launch-configuration-templates-request-schema.json
slug: application-migration-service-describe-launch-configuration-templates-request
source_filename: application-migration-service-describe-launch-configuration-templates-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-describe-launch-configuration-templates-request-schema.json\",\n  \"title\": \"DescribeLaunchConfigurationTemplatesRequest\",\n  \"description\": \"Request to describe launch configuration templates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"launchConfigurationTemplateIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by template IDs\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum results to return\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-describe-launch-configuration-templates-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: DescribeLaunchConfigurationTemplatesRequest
---
