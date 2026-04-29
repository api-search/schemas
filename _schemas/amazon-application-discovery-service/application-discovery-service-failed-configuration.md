---
description: FailedConfiguration schema from Amazon Application Discovery Service API
layout: schema
name: FailedConfiguration
properties_list:
- description: The configuration ID of the configuration that failed to delete.
  name: configurationId
  type: string
- description: The error status code.
  name: errorStatusCode
  type: integer
- description: A descriptive message indicating why the associated configuration failed to delete.
  name: errorMessage
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-failed-configuration-schema.json
slug: application-discovery-service-failed-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-failed-configuration-schema.json\",\n  \"title\": \"FailedConfiguration\",\n  \"description\": \"FailedConfiguration schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationId\": {\n      \"type\": \"string\",\n      \"example\": \"d-SERVER-500456\",\n      \"description\": \"The configuration ID of the configuration that failed to delete.\"\n    },\n    \"errorStatusCode\": {\n      \"type\": \"integer\",\n      \"example\": 404,\n      \"description\": \"The error status code.\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"example\": \"Configuration item not found\",\n      \"description\": \"A descriptive message indicating why the associated configuration failed\
  \ to delete.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-failed-configuration-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: FailedConfiguration
---
