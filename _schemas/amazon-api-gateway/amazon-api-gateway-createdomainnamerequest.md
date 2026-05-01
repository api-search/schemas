---
description: ''
layout: schema
name: CreateDomainNameRequest
properties_list:
- description: ''
  name: domainName
  type: string
- description: ''
  name: certificateName
  type: string
- description: ''
  name: certificateBody
  type: string
- description: ''
  name: certificatePrivateKey
  type: string
- description: ''
  name: certificateChain
  type: string
- description: ''
  name: certificateArn
  type: string
- description: ''
  name: regionalCertificateName
  type: string
- description: ''
  name: regionalCertificateArn
  type: string
- description: ''
  name: endpointConfiguration
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: securityPolicy
  type: string
- description: ''
  name: mutualTlsAuthentication
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createdomainnamerequest-schema.json
slug: amazon-api-gateway-createdomainnamerequest
source_filename: amazon-api-gateway-createdomainnamerequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateDomainNameRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainName\": {\n      \"type\": \"string\"\n    },\n    \"certificateName\": {\n      \"type\": \"string\"\n    },\n    \"certificateBody\": {\n      \"type\": \"string\"\n    },\n    \"certificatePrivateKey\": {\n      \"type\": \"string\"\n    },\n    \"certificateChain\": {\n      \"type\": \"string\"\n    },\n    \"certificateArn\": {\n      \"type\": \"string\"\n    },\n    \"regionalCertificateName\": {\n      \"type\": \"string\"\n    },\n    \"regionalCertificateArn\": {\n      \"type\": \"string\"\n    },\n    \"endpointConfiguration\": {\n      \"$ref\": \"#/definitions/EndpointConfiguration\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    },\n    \"securityPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TLS_1_0\",\n        \"TLS_1_2\"\n      ]\n    },\n    \"mutualTlsAuthentication\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"truststoreUri\": {\n          \"type\": \"string\"\n        },\n        \"truststoreVersion\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"domainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createdomainnamerequest-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateDomainNameRequest
---
