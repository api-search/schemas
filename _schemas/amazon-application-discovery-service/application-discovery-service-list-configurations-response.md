---
description: ListConfigurationsResponse schema from Amazon Application Discovery Service API
layout: schema
name: ListConfigurationsResponse
properties_list:
- description: Returns configuration details, including the configuration ID, attribute names, and attribute values.
  name: configurations
  type: array
- description: Token to retrieve the next set of results.
  name: nextToken
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-list-configurations-response-schema.json
slug: application-discovery-service-list-configurations-response
source_filename: application-discovery-service-list-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-list-configurations-response-schema.json\",\n  \"title\": \"ListConfigurationsResponse\",\n  \"description\": \"ListConfigurationsResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"Returns configuration details, including the configuration ID, attribute names, and attribute values.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"Token to retrieve the next set of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-list-configurations-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
title: ListConfigurationsResponse
---
