---
description: ''
layout: schema
name: ComplianceReport
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: generatedDate
  type: string
- description: Overall compliance percentage
  name: overallCompliance
  type: number
- description: ''
  name: servers
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-automation-rest-compliance-report-schema.json
slug: websphere-automation-rest-compliance-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComplianceReport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"generatedDate\": {\n      \"type\": \"string\"\n    },\n    \"overallCompliance\": {\n      \"type\": \"number\",\n      \"description\": \"Overall compliance percentage\"\n    },\n    \"servers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-automation-rest-compliance-report-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: ComplianceReport
---
