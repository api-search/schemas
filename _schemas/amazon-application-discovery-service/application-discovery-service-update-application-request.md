---
description: UpdateApplicationRequest schema from Amazon Application Discovery Service API
layout: schema
name: UpdateApplicationRequest
properties_list:
- description: Configuration ID of the application to be updated.
  name: configurationId
  type: string
- description: New name of the application to be updated.
  name: name
  type: string
- description: New description of the application to be updated.
  name: description
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-update-application-request-schema.json
slug: application-discovery-service-update-application-request
source_filename: application-discovery-service-update-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-update-application-request-schema.json\",\n  \"title\": \"UpdateApplicationRequest\",\n  \"description\": \"UpdateApplicationRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationId\": {\n      \"type\": \"string\",\n      \"example\": \"d-APP-500123\",\n      \"description\": \"Configuration ID of the application to be updated.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Production Web Tier Updated\",\n      \"description\": \"New name of the application to be updated.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Updated description for web tier servers\",\n      \"description\": \"New description of the\
  \ application to be updated.\"\n    }\n  },\n  \"required\": [\n    \"configurationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-update-application-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: UpdateApplicationRequest
---
