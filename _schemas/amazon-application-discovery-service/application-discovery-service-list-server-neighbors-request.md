---
description: ListServerNeighborsRequest schema from Amazon Application Discovery Service API
layout: schema
name: ListServerNeighborsRequest
properties_list:
- description: Configuration ID of the server for which neighbors are being listed.
  name: configurationId
  type: string
- description: Flag to indicate if port and protocol information is needed as part of the response.
  name: portInformationNeeded
  type: boolean
- description: List of configuration IDs to test for one-hop-away. Mandatory parameter when PortInformationNeeded is true.
  name: neighborConfigurationIds
  type: array
- description: Maximum number of results to return in a single page of output.
  name: maxResults
  type: integer
- description: Token to retrieve the next set of results.
  name: nextToken
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-list-server-neighbors-request-schema.json
slug: application-discovery-service-list-server-neighbors-request
source_filename: application-discovery-service-list-server-neighbors-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-list-server-neighbors-request-schema.json\",\n  \"title\": \"ListServerNeighborsRequest\",\n  \"description\": \"ListServerNeighborsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationId\": {\n      \"type\": \"string\",\n      \"example\": \"d-SERVER-500456\",\n      \"description\": \"Configuration ID of the server for which neighbors are being listed.\"\n    },\n    \"portInformationNeeded\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Flag to indicate if port and protocol information is needed as part of the response.\"\n    },\n    \"neighborConfigurationIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"\
  string\"\n      },\n      \"example\": [\n        \"d-SERVER-500457\"\n      ],\n      \"description\": \"List of configuration IDs to test for one-hop-away. Mandatory parameter when PortInformationNeeded is true.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 10,\n      \"description\": \"Maximum number of results to return in a single page of output.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"Token to retrieve the next set of results.\"\n    }\n  },\n  \"required\": [\n    \"configurationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-list-server-neighbors-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
title: ListServerNeighborsRequest
---
