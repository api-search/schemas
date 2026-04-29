---
description: DescribeConfigurationsRequest schema from Amazon Application Discovery Service API
layout: schema
name: DescribeConfigurationsRequest
properties_list:
- description: One or more configuration IDs.
  name: configurationIds
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-describe-configurations-request-schema.json
slug: application-discovery-service-describe-configurations-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-configurations-request-schema.json\",\n  \"title\": \"DescribeConfigurationsRequest\",\n  \"description\": \"DescribeConfigurationsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-SERVER-500456\"\n      ],\n      \"description\": \"One or more configuration IDs.\"\n    }\n  },\n  \"required\": [\n    \"configurationIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-configurations-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DescribeConfigurationsRequest
---
