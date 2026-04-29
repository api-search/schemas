---
description: ''
layout: schema
name: LibertyApplication
properties_list:
- description: Application name
  name: name
  type: string
- description: Application file location
  name: location
  type: string
- description: Application type
  name: type
  type: string
- description: Context root for web application
  name: contextRoot
  type: string
- description: ''
  name: state
  type: string
- description: Whether the application starts automatically
  name: autoStart
  type: boolean
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-admin-rest-liberty-application-schema.json
slug: websphere-liberty-admin-rest-liberty-application
source_filename: websphere-liberty-admin-rest-liberty-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibertyApplication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application name\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Application file location\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Application type\"\n    },\n    \"contextRoot\": {\n      \"type\": \"string\",\n      \"description\": \"Context root for web application\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"autoStart\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application starts automatically\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-admin-rest-liberty-application-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: LibertyApplication
---
