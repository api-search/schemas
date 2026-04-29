---
description: DeleteApplicationsRequest schema from Amazon Application Discovery Service API
layout: schema
name: DeleteApplicationsRequest
properties_list:
- description: Configuration ID of an application to be deleted.
  name: configurationIds
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-delete-applications-request-schema.json
slug: application-discovery-service-delete-applications-request
source_filename: application-discovery-service-delete-applications-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-delete-applications-request-schema.json\",\n  \"title\": \"DeleteApplicationsRequest\",\n  \"description\": \"DeleteApplicationsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-APP-500123\"\n      ],\n      \"description\": \"Configuration ID of an application to be deleted.\"\n    }\n  },\n  \"required\": [\n    \"configurationIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-delete-applications-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DeleteApplicationsRequest
---
