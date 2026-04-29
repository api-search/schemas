---
description: ListConfigurationsRequest schema from Amazon Application Discovery Service API
layout: schema
name: ListConfigurationsRequest
properties_list:
- description: A valid configuration identified by Application Discovery Service.
  name: configurationType
  type: string
- description: You can filter the list using a key-value format.
  name: filters
  type: array
- description: The total number of items to return. The maximum value is 100.
  name: maxResults
  type: integer
- description: Token to retrieve the next set of results.
  name: nextToken
  type: string
- description: Certain filter criteria return output that can be sorted in ascending or descending order. For a list of output characteristics for each filter, see Using the ListConfigurations Action in the AWS Appl
  name: orderBy
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-list-configurations-request-schema.json
slug: application-discovery-service-list-configurations-request
source_filename: application-discovery-service-list-configurations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-list-configurations-request-schema.json\",\n  \"title\": \"ListConfigurationsRequest\",\n  \"description\": \"ListConfigurationsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SERVER\",\n        \"PROCESS\",\n        \"CONNECTION\",\n        \"APPLICATION\"\n      ],\n      \"example\": \"SERVER\",\n      \"description\": \"A valid configuration identified by Application Discovery Service.\"\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\"\
  : \"hostName\",\n            \"description\": \"The name of the filter.\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"example\": [\n              \"server-01.example.com\"\n            ],\n            \"description\": \"A string value on which to filter.\"\n          },\n          \"condition\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"EQUALS\",\n              \"NOT_EQUALS\",\n              \"CONTAINS\",\n              \"NOT_CONTAINS\"\n            ],\n            \"example\": \"EQUALS\",\n            \"description\": \"A conditional operator. The following operators are valid \\u2014 EQUALS, NOT_EQUALS, CONTAINS, NOT_CONTAINS.\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"values\",\n          \"condition\"\n        ]\n      },\n      \"description\": \"You can filter the list using a key-value\
  \ format.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 10,\n      \"description\": \"The total number of items to return. The maximum value is 100.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"Token to retrieve the next set of results.\"\n    },\n    \"orderBy\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"example\": \"hostName\",\n            \"description\": \"The field on which to order.\"\n          },\n          \"sortOrder\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"ASC\",\n              \"DESC\"\n            ],\n            \"example\": \"ASC\",\n            \"description\": \"Ordering direction.\"\n          }\n        },\n        \"required\": [\n \
  \         \"fieldName\"\n        ]\n      },\n      \"description\": \"Certain filter criteria return output that can be sorted in ascending or descending order. For a list of output characteristics for each filter, see Using the ListConfigurations Action in the AWS Application Discovery Service User Guide.\"\n    }\n  },\n  \"required\": [\n    \"configurationType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-list-configurations-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: ListConfigurationsRequest
---
