---
description: OrderByElement schema from Amazon Application Discovery Service API
layout: schema
name: OrderByElement
properties_list:
- description: The field on which to order.
  name: fieldName
  type: string
- description: Ordering direction.
  name: sortOrder
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-order-by-element-schema.json
slug: application-discovery-service-order-by-element
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-order-by-element-schema.json\",\n  \"title\": \"OrderByElement\",\n  \"description\": \"OrderByElement schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"example\": \"hostName\",\n      \"description\": \"The field on which to order.\"\n    },\n    \"sortOrder\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ASC\",\n        \"DESC\"\n      ],\n      \"example\": \"ASC\",\n      \"description\": \"Ordering direction.\"\n    }\n  },\n  \"required\": [\n    \"fieldName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-order-by-element-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: OrderByElement
---
