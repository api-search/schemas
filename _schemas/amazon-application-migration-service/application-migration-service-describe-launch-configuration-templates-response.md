---
description: Response with launch configuration templates
layout: schema
name: DescribeLaunchConfigurationTemplatesResponse
properties_list:
- description: List of launch configuration templates
  name: items
  type: array
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-describe-launch-configuration-templates-response-schema.json
slug: application-migration-service-describe-launch-configuration-templates-response
source_filename: application-migration-service-describe-launch-configuration-templates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-describe-launch-configuration-templates-response-schema.json\",\n  \"title\": \"DescribeLaunchConfigurationTemplatesResponse\",\n  \"description\": \"Response with launch configuration templates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of launch configuration templates\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-describe-launch-configuration-templates-response-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: DescribeLaunchConfigurationTemplatesResponse
---
