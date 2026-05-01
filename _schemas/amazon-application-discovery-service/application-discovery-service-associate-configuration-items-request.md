---
description: AssociateConfigurationItemsRequest schema from Amazon Application Discovery Service API
layout: schema
name: AssociateConfigurationItemsRequest
properties_list:
- description: The configuration ID of an application with which items are to be associated.
  name: applicationConfigurationId
  type: string
- description: The ID of each configuration item to be associated with an application.
  name: configurationIds
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-associate-configuration-items-request-schema.json
slug: application-discovery-service-associate-configuration-items-request
source_filename: application-discovery-service-associate-configuration-items-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-associate-configuration-items-request-schema.json\",\n  \"title\": \"AssociateConfigurationItemsRequest\",\n  \"description\": \"AssociateConfigurationItemsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationConfigurationId\": {\n      \"type\": \"string\",\n      \"example\": \"d-APP-500123\",\n      \"description\": \"The configuration ID of an application with which items are to be associated.\"\n    },\n    \"configurationIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-SERVER-500456\"\n      ],\n      \"description\": \"The ID of each configuration item to be associated with an application.\"\
  \n    }\n  },\n  \"required\": [\n    \"applicationConfigurationId\",\n    \"configurationIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-associate-configuration-items-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
title: AssociateConfigurationItemsRequest
---
