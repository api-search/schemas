---
description: Filter schema from Amazon Application Discovery Service API
layout: schema
name: Filter
properties_list:
- description: The name of the filter.
  name: name
  type: string
- description: A string value on which to filter.
  name: values
  type: array
- description: A conditional operator. The following operators are valid — EQUALS, NOT_EQUALS, CONTAINS, NOT_CONTAINS.
  name: condition
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-filter-schema.json
slug: application-discovery-service-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"Filter schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"hostName\",\n      \"description\": \"The name of the filter.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"server-01.example.com\"\n      ],\n      \"description\": \"A string value on which to filter.\"\n    },\n    \"condition\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"EQUALS\",\n        \"NOT_EQUALS\",\n        \"CONTAINS\",\n        \"NOT_CONTAINS\"\n      ],\n      \"example\": \"\
  EQUALS\",\n      \"description\": \"A conditional operator. The following operators are valid \\u2014 EQUALS, NOT_EQUALS, CONTAINS, NOT_CONTAINS.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"values\",\n    \"condition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-filter-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: Filter
---
