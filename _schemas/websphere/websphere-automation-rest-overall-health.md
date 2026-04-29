---
description: ''
layout: schema
name: OverallHealth
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: totalServers
  type: integer
- description: ''
  name: activeServers
  type: integer
- description: ''
  name: inactiveServers
  type: integer
- description: ''
  name: openVulnerabilities
  type: integer
- description: ''
  name: criticalVulnerabilities
  type: integer
- description: ''
  name: pendingFixes
  type: integer
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-automation-rest-overall-health-schema.json
slug: websphere-automation-rest-overall-health
source_filename: websphere-automation-rest-overall-health-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OverallHealth\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"totalServers\": {\n      \"type\": \"integer\"\n    },\n    \"activeServers\": {\n      \"type\": \"integer\"\n    },\n    \"inactiveServers\": {\n      \"type\": \"integer\"\n    },\n    \"openVulnerabilities\": {\n      \"type\": \"integer\"\n    },\n    \"criticalVulnerabilities\": {\n      \"type\": \"integer\"\n    },\n    \"pendingFixes\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-automation-rest-overall-health-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: OverallHealth
---
