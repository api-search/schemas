---
description: ''
layout: schema
name: DomainName
properties_list:
- description: ''
  name: domainName
  type: string
- description: ''
  name: certificateName
  type: string
- description: ''
  name: certificateArn
  type: string
- description: ''
  name: certificateUploadDate
  type: string
- description: ''
  name: regionalDomainName
  type: string
- description: ''
  name: regionalHostedZoneId
  type: string
- description: ''
  name: regionalCertificateName
  type: string
- description: ''
  name: regionalCertificateArn
  type: string
- description: ''
  name: distributionDomainName
  type: string
- description: ''
  name: distributionHostedZoneId
  type: string
- description: ''
  name: endpointConfiguration
  type: object
- description: ''
  name: domainNameStatus
  type: string
- description: ''
  name: domainNameStatusMessage
  type: string
- description: ''
  name: securityPolicy
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: mutualTlsAuthentication
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-domainname-schema.json
slug: amazon-api-gateway-domainname
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DomainName\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainName\": {\n      \"type\": \"string\"\n    },\n    \"certificateName\": {\n      \"type\": \"string\"\n    },\n    \"certificateArn\": {\n      \"type\": \"string\"\n    },\n    \"certificateUploadDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"regionalDomainName\": {\n      \"type\": \"string\"\n    },\n    \"regionalHostedZoneId\": {\n      \"type\": \"string\"\n    },\n    \"regionalCertificateName\": {\n      \"type\": \"string\"\n    },\n    \"regionalCertificateArn\": {\n      \"type\": \"string\"\n    },\n    \"distributionDomainName\": {\n      \"type\": \"string\"\n    },\n    \"distributionHostedZoneId\": {\n      \"type\": \"string\"\n    },\n    \"endpointConfiguration\": {\n      \"$ref\": \"#/definitions/EndpointConfiguration\"\n    },\n    \"domainNameStatus\": {\n      \"\
  type\": \"string\",\n      \"enum\": [\n        \"AVAILABLE\",\n        \"UPDATING\",\n        \"PENDING\",\n        \"PENDING_CERTIFICATE_REIMPORT\",\n        \"PENDING_OWNERSHIP_VERIFICATION\"\n      ]\n    },\n    \"domainNameStatusMessage\": {\n      \"type\": \"string\"\n    },\n    \"securityPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TLS_1_0\",\n        \"TLS_1_2\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    },\n    \"mutualTlsAuthentication\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"truststoreUri\": {\n          \"type\": \"string\"\n        },\n        \"truststoreVersion\": {\n          \"type\": \"string\"\n        },\n        \"truststoreWarnings\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-domainname-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: DomainName
---
