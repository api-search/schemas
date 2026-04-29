---
description: Represents a Cloud Map namespace for service discovery.
layout: schema
name: Namespace
properties_list:
- description: The ID of the namespace.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the namespace.
  name: Arn
  type: string
- description: The name of the namespace.
  name: Name
  type: string
- description: The type of the namespace.
  name: Type
  type: string
- description: The description of the namespace.
  name: Description
  type: string
- description: The date and time that the namespace was created.
  name: CreateDate
  type: string
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-namespace-schema.json
slug: cloud-map-namespace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-namespace-schema.json\",\n  \"title\": \"Namespace\",\n  \"description\": \"Represents a Cloud Map namespace for service discovery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the namespace.\",\n      \"example\": \"ns-abc12345\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the namespace.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the namespace.\",\n      \"example\": \"production.internal\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DNS_PUBLIC\",\n        \"DNS_PRIVATE\",\n        \"HTTP\"\n      ],\n      \"description\": \"The type of the namespace.\"\
  \n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the namespace.\"\n    },\n    \"CreateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that the namespace was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-namespace-schema.json
tags:
- AWS
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: Namespace
---
