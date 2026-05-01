---
description: TagFilter schema from Amazon Application Discovery Service API
layout: schema
name: TagFilter
properties_list:
- description: A name of the tag filter.
  name: name
  type: string
- description: Values for the tag filter.
  name: values
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-tag-filter-schema.json
slug: application-discovery-service-tag-filter
source_filename: application-discovery-service-tag-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-tag-filter-schema.json\",\n  \"title\": \"TagFilter\",\n  \"description\": \"TagFilter schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"tagKey\",\n      \"description\": \"A name of the tag filter.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"environment\"\n      ],\n      \"description\": \"Values for the tag filter.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-tag-filter-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
title: TagFilter
---
