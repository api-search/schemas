---
description: DescribeContinuousExportsRequest schema from Amazon Application Discovery Service API
layout: schema
name: DescribeContinuousExportsRequest
properties_list:
- description: The unique IDs assigned to the exports.
  name: exportIds
  type: array
- description: A number between 1 and 100 specifying the maximum number of continuous export descriptions returned.
  name: maxResults
  type: integer
- description: The token from the previous call to DescribeExportTasks.
  name: nextToken
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-describe-continuous-exports-request-schema.json
slug: application-discovery-service-describe-continuous-exports-request
source_filename: application-discovery-service-describe-continuous-exports-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-continuous-exports-request-schema.json\",\n  \"title\": \"DescribeContinuousExportsRequest\",\n  \"description\": \"DescribeContinuousExportsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"continuous-export-500123\"\n      ],\n      \"description\": \"The unique IDs assigned to the exports.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 100,\n      \"example\": 10,\n      \"description\": \"A number between 1 and 100 specifying the maximum number of continuous export descriptions returned.\"\
  \n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The token from the previous call to DescribeExportTasks.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-continuous-exports-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DescribeContinuousExportsRequest
---
