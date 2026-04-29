---
description: DescribeConfigurationsResponse schema from Amazon Application Discovery Service API
layout: schema
name: DescribeConfigurationsResponse
properties_list:
- description: A key in the response map. The value is an array of data.
  name: configurations
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-describe-configurations-response-schema.json
slug: application-discovery-service-describe-configurations-response
source_filename: application-discovery-service-describe-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-configurations-response-schema.json\",\n  \"title\": \"DescribeConfigurationsResponse\",\n  \"description\": \"DescribeConfigurationsResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"A key in the response map. The value is an array of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-configurations-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DescribeConfigurationsResponse
---
