---
description: DescribeTagsRequest schema from Amazon Application Discovery Service API
layout: schema
name: DescribeTagsRequest
properties_list:
- description: You can filter the list using a key-value format. You can separate these items by using logical operators.
  name: filters
  type: array
- description: The total number of items to return in a single page of output.
  name: maxResults
  type: integer
- description: A token to start the list. Use this token to get the next set of results.
  name: nextToken
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-describe-tags-request-schema.json
slug: application-discovery-service-describe-tags-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-tags-request-schema.json\",\n  \"title\": \"DescribeTagsRequest\",\n  \"description\": \"DescribeTagsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"tagKey\",\n            \"description\": \"A name of the tag filter.\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"example\": [\n              \"environment\"\n            ],\n            \"description\": \"Values\
  \ for the tag filter.\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"values\"\n        ]\n      },\n      \"description\": \"You can filter the list using a key-value format. You can separate these items by using logical operators.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 10,\n      \"description\": \"The total number of items to return in a single page of output.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"A token to start the list. Use this token to get the next set of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-tags-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DescribeTagsRequest
---
