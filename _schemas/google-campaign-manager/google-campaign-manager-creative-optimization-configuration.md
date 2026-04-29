---
description: Creative optimization configuration.
layout: schema
name: CreativeOptimizationConfiguration
properties_list:
- description: ID of this creative optimization configuration.
  name: id
  type: string
- description: Name of this creative optimization configuration.
  name: name
  type: string
- description: List of optimization activities associated with this configuration.
  name: optimizationActivitys
  type: array
- description: Optimization model for this configuration.
  name: optimizationModel
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-creative-optimization-configuration-schema.json
slug: google-campaign-manager-creative-optimization-configuration
source_filename: google-campaign-manager-creative-optimization-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreativeOptimizationConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"Creative optimization configuration.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of this creative optimization configuration.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of this creative optimization configuration.\"\n    },\n    \"optimizationActivitys\": {\n      \"type\": \"array\",\n      \"description\": \"List of optimization activities associated with this configuration.\"\n    },\n    \"optimizationModel\": {\n      \"type\": \"string\",\n      \"description\": \"Optimization model for this configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-creative-optimization-configuration-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: CreativeOptimizationConfiguration
---
