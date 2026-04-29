---
description: ''
layout: schema
name: MBeanDetail
properties_list:
- description: ''
  name: objectName
  type: string
- description: ''
  name: className
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: attributes
  type: array
- description: ''
  name: operations
  type: array
- description: ''
  name: notifications
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-rest-connector-m-bean-detail-schema.json
slug: websphere-liberty-rest-connector-m-bean-detail
source_filename: websphere-liberty-rest-connector-m-bean-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MBeanDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"objectName\": {\n      \"type\": \"string\"\n    },\n    \"className\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"attributes\": {\n      \"type\": \"array\"\n    },\n    \"operations\": {\n      \"type\": \"array\"\n    },\n    \"notifications\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-rest-connector-m-bean-detail-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: MBeanDetail
---
