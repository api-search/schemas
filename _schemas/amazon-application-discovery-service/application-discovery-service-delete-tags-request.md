---
description: DeleteTagsRequest schema from Amazon Application Discovery Service API
layout: schema
name: DeleteTagsRequest
properties_list:
- description: A list of configuration items with tags that you want to delete.
  name: configurationIds
  type: array
- description: Tags that you want to delete from one or more configuration items.
  name: tags
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-delete-tags-request-schema.json
slug: application-discovery-service-delete-tags-request
source_filename: application-discovery-service-delete-tags-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-delete-tags-request-schema.json\",\n  \"title\": \"DeleteTagsRequest\",\n  \"description\": \"DeleteTagsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-SERVER-500456\"\n      ],\n      \"description\": \"A list of configuration items with tags that you want to delete.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"example\": \"environment\",\n            \"description\": \"The type of tag\
  \ on which to filter.\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"example\": \"production\",\n            \"description\": \"A value for a tag key on which to filter.\"\n          }\n        },\n        \"required\": [\n          \"key\",\n          \"value\"\n        ]\n      },\n      \"description\": \"Tags that you want to delete from one or more configuration items.\"\n    }\n  },\n  \"required\": [\n    \"configurationIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-delete-tags-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DeleteTagsRequest
---
