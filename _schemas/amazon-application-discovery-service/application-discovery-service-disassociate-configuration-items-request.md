---
description: DisassociateConfigurationItemsRequest schema from Amazon Application Discovery Service API
layout: schema
name: DisassociateConfigurationItemsRequest
properties_list:
- description: Configuration ID of an application from which each item is to be disassociated.
  name: applicationConfigurationId
  type: string
- description: Configuration ID of each item to be disassociated from an application.
  name: configurationIds
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-disassociate-configuration-items-request-schema.json
slug: application-discovery-service-disassociate-configuration-items-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-disassociate-configuration-items-request-schema.json\",\n  \"title\": \"DisassociateConfigurationItemsRequest\",\n  \"description\": \"DisassociateConfigurationItemsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationConfigurationId\": {\n      \"type\": \"string\",\n      \"example\": \"d-APP-500123\",\n      \"description\": \"Configuration ID of an application from which each item is to be disassociated.\"\n    },\n    \"configurationIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-SERVER-500456\"\n      ],\n      \"description\": \"Configuration ID of each item to be disassociated from an application.\"\
  \n    }\n  },\n  \"required\": [\n    \"applicationConfigurationId\",\n    \"configurationIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-disassociate-configuration-items-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DisassociateConfigurationItemsRequest
---
