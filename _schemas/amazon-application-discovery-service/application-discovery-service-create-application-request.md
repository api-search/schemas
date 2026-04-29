---
description: CreateApplicationRequest schema from Amazon Application Discovery Service API
layout: schema
name: CreateApplicationRequest
properties_list:
- description: Name of the application to be created.
  name: name
  type: string
- description: Description of the application to be created.
  name: description
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-create-application-request-schema.json
slug: application-discovery-service-create-application-request
source_filename: application-discovery-service-create-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-create-application-request-schema.json\",\n  \"title\": \"CreateApplicationRequest\",\n  \"description\": \"CreateApplicationRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Production Web Tier\",\n      \"description\": \"Name of the application to be created.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Web servers for the production environment\",\n      \"description\": \"Description of the application to be created.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-create-application-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: CreateApplicationRequest
---
