---
description: ListServerNeighborsResponse schema from Amazon Application Discovery Service API
layout: schema
name: ListServerNeighborsResponse
properties_list:
- description: List of distinct servers that are one hop away from the given server.
  name: neighbors
  type: array
- description: Token to retrieve the next set of results.
  name: nextToken
  type: string
- description: Count of distinct servers that are one hop away from the given server.
  name: knownDependencyCount
  type: integer
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-list-server-neighbors-response-schema.json
slug: application-discovery-service-list-server-neighbors-response
source_filename: application-discovery-service-list-server-neighbors-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-list-server-neighbors-response-schema.json\",\n  \"title\": \"ListServerNeighborsResponse\",\n  \"description\": \"ListServerNeighborsResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"neighbors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"sourceServerId\": {\n            \"type\": \"string\",\n            \"example\": \"d-SERVER-500456\",\n            \"description\": \"The ID of the server that opened the network connection.\"\n          },\n          \"destinationServerId\": {\n            \"type\": \"string\",\n            \"example\": \"d-SERVER-500457\",\n            \"description\": \"The ID of the server\
  \ that accepted the network connection.\"\n          },\n          \"destinationPort\": {\n            \"type\": \"integer\",\n            \"example\": 443,\n            \"description\": \"The destination network port for the connection.\"\n          },\n          \"transportProtocol\": {\n            \"type\": \"string\",\n            \"example\": \"TCP\",\n            \"description\": \"The network protocol used for the connection.\"\n          },\n          \"connectionsCount\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"example\": 125,\n            \"description\": \"The number of open network connections with the neighboring server.\"\n          }\n        },\n        \"required\": [\n          \"sourceServerId\",\n          \"destinationServerId\",\n          \"connectionsCount\"\n        ]\n      },\n      \"description\": \"List of distinct servers that are one hop away from the given server.\"\n    },\n    \"nextToken\": {\n      \"\
  type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"Token to retrieve the next set of results.\"\n    },\n    \"knownDependencyCount\": {\n      \"type\": \"integer\",\n      \"example\": 1,\n      \"description\": \"Count of distinct servers that are one hop away from the given server.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-list-server-neighbors-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
title: ListServerNeighborsResponse
---
