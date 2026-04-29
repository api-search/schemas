---
description: A Knox simple descriptor
layout: schema
name: Descriptor
properties_list:
- description: Descriptor name
  name: name
  type: string
- description: Service discovery type
  name: discoveryType
  type: string
- description: Discovery service address
  name: discoveryAddress
  type: string
- description: Cluster name
  name: cluster
  type: string
- description: Referenced provider configuration
  name: providerConfig
  type: string
- description: Services exposed by this descriptor
  name: services
  type: array
provider_name: Apache Knox
provider_slug: apache-knox
schema_file: json-schema/admin-api-descriptor-schema.json
slug: admin-api-descriptor
source_filename: admin-api-descriptor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-descriptor-schema.json\",\n  \"title\": \"Descriptor\",\n  \"description\": \"A Knox simple descriptor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Descriptor name\",\n      \"example\": \"hadoop-cluster\"\n    },\n    \"discoveryType\": {\n      \"type\": \"string\",\n      \"description\": \"Service discovery type\",\n      \"example\": \"Ambari\"\n    },\n    \"discoveryAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Discovery service address\",\n      \"example\": \"http://ambari:8080\"\n    },\n    \"cluster\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster name\",\n      \"example\": \"my-cluster\"\n    },\n    \"providerConfig\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Referenced provider configuration\",\n      \"example\": \"my-provider-config\"\n    },\n    \"services\": {\n      \"type\": \"array\",\n      \"description\": \"Services exposed by this descriptor\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-descriptor-schema.json
tags:
- API Gateway
- Authentication
- Hadoop
- Open Source
- Security
- SSO
title: Descriptor
---
