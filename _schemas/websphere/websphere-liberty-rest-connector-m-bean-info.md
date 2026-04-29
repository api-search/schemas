---
description: ''
layout: schema
name: MBeanInfo
properties_list:
- description: JMX ObjectName
  name: objectName
  type: string
- description: MBean implementation class
  name: className
  type: string
- description: MBean description
  name: description
  type: string
- description: URL for accessing this MBean's details
  name: URL
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-rest-connector-m-bean-info-schema.json
slug: websphere-liberty-rest-connector-m-bean-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MBeanInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"objectName\": {\n      \"type\": \"string\",\n      \"description\": \"JMX ObjectName\"\n    },\n    \"className\": {\n      \"type\": \"string\",\n      \"description\": \"MBean implementation class\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"MBean description\"\n    },\n    \"URL\": {\n      \"type\": \"string\",\n      \"description\": \"URL for accessing this MBean's details\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-rest-connector-m-bean-info-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: MBeanInfo
---
