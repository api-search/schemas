---
description: Tag schema from Amazon Application Discovery Service API
layout: schema
name: Tag
properties_list:
- description: The type of tag on which to filter.
  name: key
  type: string
- description: A value for a tag key on which to filter.
  name: value
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-tag-schema.json
slug: application-discovery-service-tag
source_filename: application-discovery-service-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Tag schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"environment\",\n      \"description\": \"The type of tag on which to filter.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"example\": \"production\",\n      \"description\": \"A value for a tag key on which to filter.\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-tag-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: Tag
---
