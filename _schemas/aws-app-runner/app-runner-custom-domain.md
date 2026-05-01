---
description: CustomDomain schema from AWS App Runner
layout: schema
name: CustomDomain
properties_list:
- description: ''
  name: DomainName
  type: string
- description: ''
  name: EnableWWWSubdomain
  type: boolean
- description: ''
  name: CertificateValidationRecords
  type: array
- description: ''
  name: Status
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-custom-domain-schema.json
slug: app-runner-custom-domain
source_filename: app-runner-custom-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"type\": \"string\"\n    },\n    \"EnableWWWSubdomain\": {\n      \"type\": \"boolean\"\n    },\n    \"CertificateValidationRecords\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\"\n          },\n          \"Type\": {\n            \"type\": \"string\"\n          },\n          \"Value\": {\n            \"type\": \"string\"\n          },\n          \"Status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"PENDING_VALIDATION\",\n              \"SUCCESS\",\n              \"FAILED\"\n            ]\n          }\n        }\n      }\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATING\",\n        \"CREATE_FAILED\",\n        \"ACTIVE\",\n        \"DELETING\",\n        \"DELETE_FAILED\",\n        \"PENDING_CERTIFICATE_DNS_VALIDATION\"\
  ,\n        \"BINDING_CERTIFICATE\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-custom-domain-schema.json\",\n  \"title\": \"CustomDomain\",\n  \"description\": \"CustomDomain schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-custom-domain-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: CustomDomain
---
