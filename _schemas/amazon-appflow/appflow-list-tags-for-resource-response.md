---
description: ListTagsForResourceResponse schema from Amazon AppFlow API
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: The tags used to organize, track, or control access for your flow.
  name: tags
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-list-tags-for-resource-response-schema.json
slug: appflow-list-tags-for-resource-response
source_filename: appflow-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"ListTagsForResourceResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"environment\": \"production\",\n        \"team\": \"data-engineering\"\n      },\n      \"description\": \"The tags used to organize, track, or control access for your flow.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-tags-for-resource-response-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ListTagsForResourceResponse
---
