---
description: Specification for creating a new conformance scan job
layout: schema
name: JobSpec
properties_list:
- description: On-premises scan token issued by the 42Crunch Platform
  name: token
  type: string
- description: ''
  name: name
  type: object
- description: Expiration time for the job in seconds (max 7 days)
  name: expirationTime
  type: integer
- description: Hostname and port for connecting to the 42Crunch Platform
  name: platformService
  type: string
- description: Docker image for the scand-agent container
  name: scandImage
  type: string
- description: Environment variables for scand-agent. Must start with SECURITY_, SCAN42C_, HTTP_PROXY, HTTPS_PROXY, HTTP_PROXY_API, HTTPS_PROXY_API, NO_PROXY, or NO_PROXY_API.
  name: env
  type: object
provider_name: 42Crunch
provider_slug: 42crunch
schema_file: json-schema/scand-manager-job-spec-schema.json
slug: scand-manager-job-spec
source_filename: scand-manager-job-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-job-spec-schema.json\",\n  \"title\": \"JobSpec\",\n  \"description\": \"Specification for creating a new conformance scan job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"description\": \"On-premises scan token issued by the 42Crunch Platform\",\n      \"type\": \"string\",\n      \"pattern\": \"^(scan_)?[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$\",\n      \"maxLength\": 41,\n      \"minLength\": 36,\n      \"example\": \"00000000-0000-0000-0000-000000000000\"\n    },\n    \"name\": {\n      \"$ref\": \"#/components/schemas/JobName\"\n    },\n    \"expirationTime\": {\n      \"description\": \"Expiration time for the job in seconds (max 7 days)\",\n      \"type\": \"integer\",\n      \"maximum\": 604800,\n      \"minimum\": 1,\n \
  \     \"format\": \"int32\",\n      \"example\": 3600\n    },\n    \"platformService\": {\n      \"description\": \"Hostname and port for connecting to the 42Crunch Platform\",\n      \"type\": \"string\",\n      \"pattern\": \"^[^:]+:[0-9]{3,5}$\",\n      \"maxLength\": 128,\n      \"minLength\": 3,\n      \"example\": \"protection.42crunch.com:8001\"\n    },\n    \"scandImage\": {\n      \"description\": \"Docker image for the scand-agent container\",\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\P{Cc}{1,128}$\",\n      \"maxLength\": 128,\n      \"minLength\": 1,\n      \"example\": \"42crunch/scand-agent:latest\"\n    },\n    \"env\": {\n      \"description\": \"Environment variables for scand-agent. Must start with SECURITY_, SCAN42C_, HTTP_PROXY, HTTPS_PROXY, HTTP_PROXY_API, HTTPS_PROXY_API, NO_PROXY, or NO_PROXY_API.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"pattern\": \"^\\\\P{Cc}+$\",\n        \"minLength\"\
  : 0,\n        \"maxLength\": 512\n      },\n      \"example\": {\n        \"HTTPS_PROXY\": \"http://proxy.example.com:8080\",\n        \"HTTPS_PROXY_API\": \"http://proxy-api.example.com:8080\",\n        \"SECURITY_FOO\": \"bar\",\n        \"SCAN42C_FEATURE_FLAG\": \"enabled\"\n      }\n    }\n  },\n  \"additionalProperties\": false,\n  \"required\": [\n    \"token\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/42crunch/refs/heads/main/json-schema/scand-manager-job-spec-schema.json
tags:
- API Security
- Platform
- Scanning
- Security
- OpenAPI
- DevSecOps
title: JobSpec
---
