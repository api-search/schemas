---
description: ''
layout: schema
name: CreateDomainAssociationRequest
properties_list:
- description: ''
  name: domainName
  type: string
- description: ''
  name: subDomainSettings
  type: array
provider_name: Amazon Amplify
provider_slug: amazon-amplify
schema_file: json-schema/amazon-amplify-createdomainassociationrequest-schema.json
slug: amazon-amplify-createdomainassociationrequest
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateDomainAssociationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainName\": {\n      \"type\": \"string\"\n    },\n    \"subDomainSettings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"prefix\": {\n            \"type\": \"string\"\n          },\n          \"branchName\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"domainName\",\n    \"subDomainSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-amplify/refs/heads/main/json-schema/amazon-amplify-createdomainassociationrequest-schema.json
tags:
- AWS
- Frontend
- Full Stack
- Hosting
- Mobile Development
- Web Applications
title: CreateDomainAssociationRequest
---
