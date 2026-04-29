---
description: Request to enable template list information for the client.
layout: schema
name: Enable_Template_Info_Post
properties_list:
- description: Template ID
  name: tmpl_id
  type: string
- description: Template name
  name: tmpl_name
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-bookbuilder-enable_template_info_post-schema.json
slug: factset-bookbuilder-enable_template_info_post
source_filename: factset-bookbuilder-enable_template_info_post-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Enable_Template_Info_Post\",\n  \"type\": \"object\",\n  \"description\": \"Request to enable template list information for the client.\",\n  \"properties\": {\n    \"tmpl_id\": {\n      \"type\": \"string\",\n      \"description\": \"Template ID\"\n    },\n    \"tmpl_name\": {\n      \"type\": \"string\",\n      \"description\": \"Template name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-bookbuilder-enable_template_info_post-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Enable_Template_Info_Post
---
